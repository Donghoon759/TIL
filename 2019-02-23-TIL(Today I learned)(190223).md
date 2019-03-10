---
layout: post
title: "TIL(Today I learned)(190223)"
date: 2019-02-23
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

- npm 개념 익히기
	- Node Package Manager
	- 패키지를 관리하도록 도와준다.
	- package.json으로 관리
	- 패키지 하나가 다른 여러 패키지에 의존하고, 그 패키지들이 또 다른 패키지들에 의존하므로 이렇게 관리가 필요하다.
	- npm install express -> express를 해당 폴더에 다운로드
	- npm install express --save -> express를 다운로드하고 package.json에 등록
	- g 옵션 : 프로그램을 컴퓨터에 global로 다운로드 하는 것으로, 해당폴더에 설치 안되고, package.json에도 등록안된다.
	- nodemon이라는 tool을 global로 설치했다.(코드가 수정되면 서버를 알아서 재실행해줌)

- 게시판 프로젝트의 기본 세팅
	- package.json을 작성하고 express를 설치했다.
	- app.js에서 다른 모듈들을 가져오고 기본적인 라우팅 설정을 했다.

- git 명령어
	- git remote show [리모트 저장소 이름] : 리모트 저장소의 구체적인 정보 확인

[참고 블로그]
(https://blog.naver.com/PostView.nhn?blogId=azure0777&logNo=220465552731&parentCategoryNo=&categoryNo=18&viewDate=&isShowPopularPosts=false&from=postView)
