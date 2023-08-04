# How to contribute to Tech Blog

이 가이드는 기고자가 직접 마크다운과 Material for MkDocs 라이브러리를 활용하여 테크 블로그에 기고하는 방법을 안내합니다.

안내 범위는 기획안을 바탕으로한 초안 템플릿 생성부터 초안 배포까지이며 그외 전체적인 블로그 운영 프로세스는 여기를 참고하세요.

당신이 기고자인 경우, Step 2 중심으로 확인하시기 바랍니다.


## Step 1: TW가 초안 템플릿 생성
TW가 초안 작성을 위한 feature 브랜치 생성 후 기획안을 바탕으로  초안 템플릿을 작성합니다.

develop 브랜치를 기준으로 feature 브랜치 생성 후 초안 템플릿 작업 --> feature 브랜치 공유


## Step 2: 기고자가 초안 작성 

1. 문서 작업 환경 구성
기고자의 로컬 환경에서 블로그와 동일한 사이트를 빌드하며 초안 작성을 할 수 있도록 아래 순서대로 작업 환경을 구성합니다.


```
python.exe -m pip install --upgrade pip
python.exe -m pip install  mkdocs-material
python.exe -m pip install git+https://{PAT}@github.com/morai-techblog/mkdocs-material-insiders.git

pip install mkdocs-minify-plugin
pip install mkdocs-rss-plugin
```

2. 블로그 리포지터리 복사 

`git clone --branch <feature branchname> https://github.com/morai-techblog/morai-techblog.github.io.git`

3. 초안 작성 
초안 템플릿의 각 주요 항목에 대한 내용을 채운다는 개념으로 작성.  
각 목차 및 단락 별 소주제에 맞는 내용을 작성하는 것이 중요함. 이에 필요한 캡처, 표, 그림을 최대한 활용하여 포함

초안 작성 후 1차 맞춤법 검사 --> [다음 맞춤법 검사기](https://alldic.daum.net/grammar_checker.do)

4. 초안 공유

feature 브랜치 업데이트 

git commit -am "초안 작성 완료"

git push origin {feature branch}


## Step 3: TW가 초안 수정 및 편집

TW가 feature 브랜치 업데이트 후 develope 브랜치에 머지하도록 PR  요청 (meta.draft: true 상태)

기고자가 머지 승인 및 머지 완료


## Step 4: 초안 완성 및 배포

TW가 메타 데이터 확정: 날짜, 작가, 제목, 설명, 카테고리 등 (meta.draft: false로 변경),최종 내용 검수

TW가 PR 요청: develop --> main branch, 

Github Action 으로 맞춤법 자동 검사 

PM이 코멘트 후 머지 승인, 머지 완료

TW가 gh-pages  브랜치에 초안 배포: 
`mkdocs gh-deploy --config-file mkdocs.yml --remote-branch gh-pages`






