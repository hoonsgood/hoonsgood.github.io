---
layout: single

title: "GitHub Pages 만들기"
excerpt: ""

date: 2021-08-10 01:46:00 +0900
lastmod: 2021-08-10 01:51:00 +0900 # sitemap.xml에서 사용됨

author_profile: true # 왼쪽부분 프로필을 띄울건지

categories: 
  - github.io

tags: 
    - github.io
---

## 1. 테마 선택
[Jekyll theme](https://github.com/topics/jekyll-theme) 링크를 통해 마음에 드는 테마를 선택한다.\
## 2. fork
테마에 대한 github page 우측 상단의 `fork` 버튼을 클릭한다.\
해당 테마의 전체 소스가 내 github 계정으로 복사가 된 것을 확인한다.
## 3. GitHub Pages 설정
### Rename
복사된 테마의 `Settings`에서 `Repository name`을 변경한다.\
`Repository name`은 반드시 `{github 계정}.github.io`을 설정해야한다.
### _config.yml 설정
`url` 설정을 위에서 변경한 `https://Repository name`으로 변경한다.
## 4. post 하기
`_posts` 폴더 아래에 블로그 글을 발행을 한다.\
블로그 글을 쓸때에는 아래 규칙을 따라야 한다.\
File name : yyyy-MM-dd-title.md\
File first line : 
```
---
slayout: simple
title:  "Welcome to Jekyll!"
---
```



