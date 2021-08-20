---
layout: single

title: "Troubleshooting node-gyp, windows-build-tools"
excerpt: ""

date: 2021-08-14 02:55:00 +0900
lastmod: 2021-08-14 02:55:00 +0900 # sitemap.xml에서 사용됨

author_profile: true # 왼쪽부분 프로필을 띄울건지

categories: 
  - css

tags: 
    - troubleshooting
    - nodejs
    - node-gyp
---
npm으로 네이티브 모듈 설치 중 빌드 에러 발생 시, 아래와 같이 진행한다.

## 1. windows-build-tools가 설치되어 있다면 삭제
## 2. node-gyp가 설치되어 있다면 삭제
## 3. python 2.7.x버전 설치 후 환경변수 등록
## 4. Powershell을 관리자 권한으로 열어 아래 모듈 설치
```bash
$ npm install --global --production windows-build-tools@4.0.0
$ npm install --global node-gyp
```
## 5. npm config 설정
```bash
$ npm config set python C:\Python27
$ npm config set msvs_version 2015 –global
```

이후에 npm install을 하면 정상적으로 설치가 되었다.