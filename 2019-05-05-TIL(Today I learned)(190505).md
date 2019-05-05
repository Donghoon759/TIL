---
layout: post
title: "TIL(Today I learned)(190505)"
date: 2019-05-05
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

- React 공부
	- Immutable.js
		- 데이터구조 Map을 사용
		- 내부 객체도 Map을 사용
		- fromJS를 사용하면 내부 객체들은 Map을 쓰지 않아도 된다.
	- toJS로 일반 객체 형태로 변형
	- get으로 특정 키 값 불러옴
	- getIn으로 Map안의 Map을 불러옴
	- set으로 새 값 설정