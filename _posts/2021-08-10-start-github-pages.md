---
slayout: simple
title:  "GitHub Pages 만들기"
---

# GitHub Pages 만들기
## 1. 테마 선택
[Jekyll theme](https://github.com/topics/jekyll-theme) 링크를 통해 마음에 드는 테마를 선택합니다.\
Star가 많을수록 인기있는 테마입니다.
## 2. fork
테마에 대한 github page 우측 상단의 `fork` 버튼을 클릭합니다.\
해당 테마의 전체 소스가 내 github 계정으로 복사가 된 것을 확인합니다.
## 3. GitHub Pages 설정
### Rename
복사된 테마의 `Settings`에서 `Repository name`을 변경합니다.\
`Repository name`은 반드시 `{github 계정}.github.io`을 설정해야합니다.
### _config.yml 설정
`url` 설정을 위에서 변경한 `https://Repository name`으로 변경합니다.
## 4. post 하기
`_posts` 폴더 아래에 블로그 글을 발행을 합니다.
블로그 글을 쓸때에는 아래 규칙을 따라야 합니다.
File name : yyyy-MM-dd-title.md\
File first line : 
```
---
slayout: simple
title:  "Welcome to Jekyll!"
---

```



