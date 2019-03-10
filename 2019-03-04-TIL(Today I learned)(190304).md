---
layout: post
title: "TIL(Today I learned)(190304)"
date: 2019-03-04
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

- nodejs 교과서 프로젝트 9장 마무리!

- 데이터베이스에 한글 세팅이 안되어 있어서 오류가 났다.
	- 15장 sequelize 세팅을 참고하여 한글 세팅을 함.

- npm에서 pkg 모듈이 dependencies들을 추가해 준다는 것을 알았다.

- 디지털 신호 전송 시 Baseband와 Broadband 방식의 차이
	- Baseband
		- 변조없이 그대로 전송.(모뎀이 필요없음)
		- 근거리 전송에 주로 사용, 구성이 간단함.
		- 네트워크 운영 비용이 저렴.
		- 양방향 전송이 가능
		- 장거리 전송에 부적합
		- 통신 잡음에 쉽게 변형되어서 손실이 큼.
	- Broadband
		- 디지털 신호를 여러 개의 신호로 변조 후 다른 주파수 대역응로 동시에 전송.
		- 장거리 전송에 주로 사용.
		- 잡음에 의한 신호감소가 적음.
		- 다중 채널을 이용해 영상, 음성 등을 전송
		- 회로가 매우 복잡해 설치 및 관리가 어려움
		- 단방향 전송