---
layout: post
title: "TIL(Today I learned)(190128)"
date: 2019-01-28
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


- Node.js 교과서 3.5장 노드 내장 모듈 사용하기 파트를 공부했다.
	- 노드는 웹 상의 자바스크립트와는 달리 os 모듈을 사용해 운영체제의 정보를 가져올 수 있다.
	- 폴더와 파일의 경로를 쉽게 조작할 수 있게 해주는 path 모듈이 있다.
	- 인터넷 주소를 쉽게 조작하도록 해주는 url 모듈이 있다.
	- 기존 노드의 url을 사용할 때 search 부분을 사용하기 쉽게 객체로 만드는 querystring 모듈이 있다.
	- 다양한 방식의 암호화를 도와주는 crypto 모듈이 있다.
	- 각종 편의 기능을 모아둔 util 이라는 모듈이 있다.
		- util 모듈에서 deprecate, promisify 메서드를 자주 사용한다.  
- Java로 재귀 알고리즘을 공부했다.
	- Factorial 함수와 최댓값 구하기 함수를 재귀, 비재귀로 구현해보았다.  

- Jekyll 공부를 했다.
	- 오늘 내 블로그에 google-analytics 기능을 활성화했다.
		- google-analytics 기능은 아직 정확히 무슨 기능인지 몰라서 더 찾아볼 예정이다.
	- disqus를 활용한 comment 기능도 활성화했고 실제로 포스트에서 작동하는 것을 확인했다.
		- 실제 내 블로그 글 밑에 comment를 다는 창이 추가된 것을 확인했다.
		- disqus가 동작하게 해주는 코드를 봤는데 javascript 코드로 이루어져있었고 disqus 설정에서 얻은 shortname을 변수로 설정해주었더니 동작하였다. 이 과정은 추후 포스트로 올려볼 생각이다.  