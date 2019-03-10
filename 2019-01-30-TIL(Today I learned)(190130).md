---
layout: post
title: "TIL(Today I learned)(190130)"
date: 2019-01-30
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title/
comments: true
tag: TIL
---


## Node.js
- 4.1장 요청과 응답 이해하기,
	- 클라이언트에서 서버로 요청을 보내고 서버에서는 요청에 응답을 한다.
	- 웹 브라우저의 요청을 처리하도록 http 모듈을 사용해 http 서버를 구축한다.
	- createServer 메서드 뒤에 listen 메서드를 붙이고 연결 완료 후 실행될 콜백 함수도 넣어준다.
	- Localhost는 컴퓨터 내부주소로, 외부에서는 접근불가하며, 포트번호를 80번을 사용하면 생략할 수 있다.
	- 응답 시 클라이언트에게 문자열이나 버퍼를 보내줄 수 있다.  


- 4.2장 쿠키와 세션 이해하기
	- 쿠키는 이용자가 누군지 식별하게 해주는 작은 데이터 조각
	- 요청 -> 쿠키와 함께 응답 -> 쿠키와 함께 요청 -> 응답
	- 쿠키는 요청과 응답의 헤더에 저장, 키-값의 쌍
	- 옵션 값
		- 쿠키명=쿠키값
		- Expires=날짜(만료 기한)
		- Max-age=초(해당 초가 지나면 쿠키 제거, Expires보다 우선)
		- Domain=도메인명(쿠키가 전송될 도메인, 기본값은 현재 도메인)
		- Path=URL(쿠키가 전송될 URL, 기본값은 '/')
		- Secure(HTTPS일 경우에만 쿠키 전송)
		- HttpOnly(자바스크립트에서 쿠키 접근불가, 쿠키 조작 방지)
	- 그 외 헤더에 대해서 공부
		- 공용 헤더(요청과 응답 둘 다 해당)
		- 요청 헤더
		- 응답 헤더
		- CORS Problem
		- 쿠키와 캐시의 전용 헤더  

---
## DP(동적계획법)
DP는 DP처럼 풀기 위해 노력하자.  

---
[온라인 코딩 사이트 REPL](https://repl.it)