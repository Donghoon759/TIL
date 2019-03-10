---
layout: post
title: "TIL(Today I learned)(190308)"
date: 2019-03-08
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


- Nodejs API 서버 만들기 시작
	-	npm bcrypt install 오류 해결
	-	jwt 토큰으로 사용자 인증하기 구현

sudo npm install bcrypt
bcrypt package를 install하다가 다음과 같은 에러를 만났다.

https://github.com/npm/npm/issues/17268

`sudo npm install bcrypt --unsafe-perm=true`를 사용