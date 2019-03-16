---
layout: post
title: "TIL(Today I learned)(190316)"
date: 2019-03-16
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

## Node
### Node.js 사용의 장점
- Node.js 패키지 매니저의 모듈들
- 비동기 I/O
	- 비동기 입출력을 효과적으로 처리할 수 있다.
- 활발한 커뮤니티
- 일체형과 마이크로서비스

## Database command
### CREATE DATABASE A default CHARACTER SET UTF8;
A라는 데이터베이스를 만들고 한글을 사용할 수 있는 UTF8로 문자열을 저장

## Git commands
### git push origin login
login이라는 local branch를 원격 저장소로 push

### git remote show origin
원격 브랜치 내역 확인

### git push origin :login
login remote branch 삭제

### git push origin login:master
local branch login에서 remote branch master로 push한다.

### git push --set-upstream origin login
현재 branch의 upstream을 origin이라는 remote branch의 login remote branch로 설정한다.