---
date: 2023-07-14
authors: 
  - EJ
description: Github Action의 자동 맞춤범 검사기를 도입하여 개발자가 초안을 빠르게 수정하기
categories:
  - Cases Study
cover_image: post_230714.png
title: 맞춤법 자동검사 도입기 feat. 마크다운 사용법
draft: true
comments: true
---

# 제목: TEST
안녕하세요. OOO에서 OO을 하고 있는 OOO 입니다.

## TEST
아래의 잘못된 맞춤법이 Github Action으로 고쳐졌을까요?

- 써버
- 쓰레드
- 캐쉬
- 푸쉬
- 크래쉬
- 아키텍쳐
- 리젼
- 챠트
- 디렉토리
- 리포지토리
- 웹 사이트
- 어플리케이션
- 메뉴얼
- 드랍
- 애뮬레이터
- 라이센스
- 매니패스트
- 맵핑
- 메세지
- 릴리즈
- 스케쥴
- 쉘
- 버츄얼
- 썸네일
- 버젼
- 프로비젼

## 맞춤법 오류 추가2
- 써버
- 쓰레드

## 맞춤법 오류 추가 2
- 서버
- 스레드
- 캐쉬
- 푸쉬
- 크래쉬
- 아키텍쳐
- 리젼
- 챠트
- 디렉토리
- 리포지토리
- 웹 사이트
- 어플리케이션
- 메뉴얼
- 드랍
- 애뮬레이터
- 라이센스
- 매니패스트
- 맵핑
- 메세지
- 릴리즈
- 스케쥴
- 쉘
- 버츄얼


### 맞춤법 오류 추가 2
- 서버 by github action
- 스레드 by github action
- 캐쉬 -> 캐시
- 푸쉬 -> 푸쉬
- 크래쉬 -> 크래시
- 아키텍쳐 -> 아키텍처
- 리젼 -> 리전
- 챠트 -> 차트
- 디렉토리 -> 디렉터리
- 리포지토리 -> 리파지터리
- 웹 사이트 -> 웹사이트
- 어플리케이션 -> 애플리케이션
- 메뉴얼 -> 매뉴얼
- 드랍 -> 드롭
- 애뮬레이터 -> 에뮬레이터
- 라이센스 -> 라이선스
- 매니패스트 -> 매니페스트
- 맵핑 -> 매핑
- 메세지 -> 메시지
- 릴리즈 -> 릴리스
- 스케쥴 -> 스케줄
- 쉘 -> 셸
- 버츄얼 -> 버추얼

---

##  마크다운 사용법

#### 안내사항
???+ note
    Capture Mode는 센서 설정 파라미터로 **GT** 및 **Intensity Type** 을 지원하는 카메라 및 라이다 센서에서만 사용할 수 있습니다.

#### 코드 블록
``` yaml
site_name: My Blog
theme:
  name: material
  features:
    - navigation.sections
plugins:
  - meta
  - blog:
      blog_dir: . 
  - search
  - tags
nav:
  - index.md
```

#### 일반 설명 블록 
To use multiple sensors in MORAI SIM: Air, the system specifications below should be satisfied.
>  CPU: Intel i7 or higher <br>
  RAM: 32GB  or higher <br>
>  VGA: RTX 30 series or higher
>

#### 리스트형 일반 설명 블록 
To use multiple sensors in MORAI SIM: Air, the system specifications below should be satisfied.
> - CPU: Intel i7 or higher <br>
  - RAM: 32GB  or higher <br>
> - VGA: RTX 30 series or higher


#### 두 개 이상 열 리스트
<div class="mdx-columns" markdown>

- [Adding an excerpt]
- [Adding authors]
- [Adding categories]
- [Adding tags]
- [Adding related links]
- [Linking from and to posts]
- [Setting the reading time]
- [Setting defaults]

</div>

  [exact same Markdown flavor]: ../../reference/index.md
  [post slugs]: ../../setup/setting-up-a-blog.md#+blog.post_url_format
  [draft]: ../../setup/setting-up-a-blog.md#drafts
  [This behavior can be changed]: ../../setup/setting-up-a-blog.md#+blog.draft
  [live preview server]: ../../creating-your-site.md#previewing-as-you-write
  [archive]: ../../setup/setting-up-a-blog.md#archive
  [category]: ../../setup/setting-up-a-blog.md#categories
  [Blog]: blog-support-just-landed/blog.png
  [Blog post]: blog-support-just-landed/blog-post.png
  [Adding an excerpt]: ../../setup/setting-up-a-blog.md#adding-an-excerpt
  [Adding authors]: ../../setup/setting-up-a-blog.md#adding-authors
  [Adding categories]: ../../setup/setting-up-a-blog.md#adding-categories
  [Adding tags]: ../../setup/setting-up-a-blog.md#adding-tags
  [Adding related links]: ../../setup/setting-up-a-blog.md#adding-related-links
  [Linking from and to posts]: ../../setup/setting-up-a-blog.md#linking-from-and-to-posts
  [Setting the reading time]: ../../setup/setting-up-a-blog.md#setting-the-reading-time
  [Setting defaults]: ../../setup/setting-up-a-blog.md#setting-defaults
  [configuration options]: ../../setup/setting-up-a-blog.md#configuration

#### 번호형 리스트

1.  [Subscribe to a monthly sponsorship]
2.  [Create a personal access token]
3.  [Install Insiders]

#### 주석형 코드 블록
Now that we have set up the [built-in blog plugin], we can start writing our
first post. All blog posts are written with the [exact same Markdown flavor] as
already included with Material for MkDocs. First, create a folder called `posts`
with a file called `hello-world.md`:

``` { .sh .no-copy }
.
├─ docs/
│  ├─ posts/
│  │  └─ hello-world.md # (1)!
│  └─ index.md
└─ mkdocs.yml
```

1.  If you'd like to arrange posts differently, you're free to do so. The URLs
    are built from the format specified in [`post_url_format`][post slugs] and
    the titles and dates of posts, no matter how they are organized
    inside the `posts` directory.

Then, open up `hello-world.md`, and add the following lines:

``` yaml
---
draft: true # (1)!
date: 2022-01-31
categories:
  - Hello
  - World
---
```

## 결론
결론입니다.
