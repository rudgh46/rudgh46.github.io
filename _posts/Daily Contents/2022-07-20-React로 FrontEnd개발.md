---
title: "[React로 FrontEnd 개발해보기]"
categories:
  - Daily Contents
tags:
  - Daily Contents
  # -
toc: true
toc_sticky: true
toc_label: "React로 FrontEnd 개발해보기"
toc_icon: "bookmark"
---

<br>

# React

## 설치 및 시작

1. Nodejs 설치 : npm(Node Package Manager)
2. CRA 설치 : 설치 희망 path > npx create-react-app testpjt

```
- npm = npx
- npm이 버전업이 되면서 나온 명령어
```

** npm start 로 실행!! **

- App.js : 모든 소스가 있는 곳

- index.html, index.js

  - index.js 파일의 root.render 라는 렌더링 선언, 그 내부의 App라는 커스터마이징된 태그가 컴포넌트.
  - App.js가 SPA를 위해 injection 되어있다.
  - App.js의 내부 function 등의 내용 수정에 따라 페이지의 내용이 변경.

## 테이블 생성 & 데이터 적용

- React 문법 : 대부분의 Object 표현 방식
- { } 중괄호 활용. ex) let title = ['이름', '전공'] => { title[0] }

## useState

- import { useState } from 'react';

```
[객체, 대체값]
let[name, nameUpdate] = useState['이름1', '이름2'];
=> button onClick {() => { nameUpdate(['이름3', '이름4']) } }

앞의 name은 대표하는 변수명, 뒤의 nameUpdate는 대체할 수 있는 값.
=> 아래의 버튼으로 원래의 이름1, 이름2를 이름3, 이름4로 바꾸는 것이 가능.
```

## component

- ex) function TrComp(props)
- 상위 컴포넌트에서 name과 major 등의 미리 정해둔 변수값을 props를 통해 하위 컴포넌트로 전함.

## DataGrid

- import { DataGrid } from '@mui/x-data-grid';
- json 형태로 만들어둔 값을 <DataGrid rows={rows} columns={columns} /> 등으로 주입.

## DataGrid 응용

- API 활용하여 응용
- ex) <DataGrid rows={rows} columns={columns} rowsPerPageOptions={[13,26,100]} checkboxSelection />
