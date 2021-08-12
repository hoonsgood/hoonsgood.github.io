---
layout: single

title:  "minimal mistakes theme 네비게이션 설정"
excerpt: ""

date: 2021-08-12 20:17:00 +0900
lastmod: 2021-08-12 20:17:00 +0900 # sitemap.xml에서 사용됨

author_profile: false # 왼쪽부분 프로필을 띄울건지

header:
  overlay_image: https://images.unsplash.com/photo-1501785888041-af3ef285b470?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80
  overlay_filter: 0.5 # 투명도

categories: 
  - github io

tags: 
    - github io
    - theme
    - front matter

# table of contents
toc: true # 오른쪽 부분에 목차를 자동 생성해준다.
toc_label: "table of content" # toc 이름 설정
toc_icon: "bars" # 아이콘 설정
toc_sticky: true # 마우스 스크롤과 함께 내려갈 것인지 설정
---

# _pages 디렉토리 생성
네비게이션을 사용하기 위해 루트 디렉토리에 _page 디렉토리를 생성하고, `docs/_pages` 경로로 들어가서 하단 목록의 파일들을 루트폴더의 `_pages`로 가져온다.

`docs/_pages/404.md`\
`docs/_pages/category-archive.md`\
`docs/_pages/tag-archive.md`\
`docs/_pages/year-archive.md`\

# 네비게이션 항목 추가
`_date` 디렉토리의 `navigation.yml`을 아래와 같이 수정합니다.
```
main:
  - title: "About"
    url: /about/
  - title: "Category"
    url: /categories/
  - title: "Tag"
    url: /tags/
  - title: "Archive"
    url: /year-archive/
```

# 불필요한 파일 및 폴더 삭제
- .editorconfig
- .gitattributes
- .github
- /docs
- /test
- CHANGELOG.md
- minimal-mistakes-jekyll.gemspec
- README.md
- screenshot-layouts.png
- screenshot.png

