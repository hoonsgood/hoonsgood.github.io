---
layout: single

title:  "minimal mistakes theme 네비게이션 설정"
excerpt: ""

date: 2021-08-12 01:50:00 +0900
lastmod: 2021-08-12 01:50:00 +0900 # sitemap.xml에서 사용됨

author_profile: true # 왼쪽부분 프로필을 띄울건지

categories: 
  - github io

tags: 
    - github io
    - theme
    - navigation
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

