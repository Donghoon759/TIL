---
layout: post
title: "TIL(Today I learned)(190402)"
date: 2019-04-02
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

docker -v
도커 엔진 버전확인

docker pull
docker hub로부터 이미지 다운로드

docker images
도커 엔진에 존재하는 이미지 출력

docker create -i -t --name mycentos centos:7
컨테이너의 이름을 mycentos로 설정

docker attach
컨테이너 내부로 들어가는 것

docker start
컨테이너 실행

docker create
이미지가 없으면 docker pull -> docker create

docker run
이미지가 없으면 docker pull -> docker create -> docker start -> docker attach(-it 옵션을 사용했을때)

docker start ID(3~4자)
리눅스에서 tab을 누르는 것과 같은 효과

docker ps
정지되지 않은 컨테이너만 출력

docker ps -a
컨테이너 전부 출력

docker ps -q
컨테이너의ID만 출력

docker inspect

컨테이너가 시작될때 실행되는 COMMAND명령어는 대부분 내장되어있다.

docker run -it ubuntu:14.04 echo hello world!
-> 이런식으로 덮어쓸 수 있다.
-> 위 컨테이너는 실행될 때마다 "echo hello world!"를 실행한다.
-> 이는 /bin/bash를 덮어쓰기 때문에 상호 입출력이 가능한 셸이 실행되지 않으니 출력만하고 컨테이너가 종료된다.

docker rename
컨테이너의 이름을 변경

docker rm
컨테이너 삭제
-f붙이면 실행중인 것도 삭제

docker stop
컨테이너 중지

docker container prune
컨테이너 모두 삭제

컨테이너는 가상 머신과 마찬가지로 가상 IP 주소를 할당받는다.

ifconfig
컨테이너의 네크워크 인터페이스 확인

컨테이너는 설정없이 외부에서 접근할 수 없으며 도커가 설치된 호스트에서만 접근할 수 있다.
eth0의 IP와 포트를 호스트의 IP와 포트에 바인딩해야 외부에 노출된다.

docker run -it --name mywebserver <b>-p 80:80</b> ubuntu:14.04
호스트의 포트:컨테이너의 포트

docker run -it -p 3306:3306 -p 192.168.0.100:7777:80 ubuntu:14.04
이것 처럼 여러개도 가능

아파치 웹 서버는 172 대역을 가진 컨테이너의 NAT IP와 80번 포트로 서비스한다.

한 컨테이너에 프로세스 하나만 실행하는 것이 도커의 철학



