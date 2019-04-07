---
layout: post
title: "TIL(Today I learned)(190407)"
date: 2019-04-07
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

데이터 링크 계층 : 이더넷 규칙 기반

- 같은 네트워크에 있는 컴퓨터로 데이터 전송 가능
- 인터넷이나 다른 네트워크로는 데이터 전송 불가

네트워크계층의 역할 : 네트워크 간의 통신을 가능하게 한다.

다른 네트워크로 데이터를 전송하려면 라우터가 필요

- 가정이나 소규모 기업 용도로 만든 라우터 : 인터넷 공유기
- 라우터는 데이터의 목적지가 정해지면 해당 목적지까지 어떤 경로로 가는 것이 좋은지 알려준다.
- 라우팅(routing) : 목적지 IP 주소까지 어떤 경로로 데이터를 보낼지 결정
- 거리에 관계없이 다른 네트워크로 데이터를 보낼 수 있다.
- 라우팅 테이블(routing table) : 경로 정보를 등록하고 관리

IP주소 : 네트워크를 식별하는 주소

- 어떤 네트워크의 어떤 컴퓨터인지를 구분할 수 있도록 한다.

## IP(Internet Protocol)

- 네트워크 계층에서 IP프로토콜을 사용해서 캡슐화할 때 IP 헤더를 붙인다.
    - 버전(version)
    - 헤더 길이(header length)
    - 서비스 유형(service type)
    - 전체 패킷 길이(total length)
    - ID (identification, 일련 번호)
    - 조각 상태(flags)
    - 조각의 위치(fragment offset)
    - TTL
    - 프로토콜(protocol)
    - 헤더 체크섬(header checksum)
    - 출발지 IP주소(source IP address)
    - 목적지 IP주소(destination IP address)
- 이렇게 만들어진 것 → IP 패킷

## 정리

- 서로 다른 네트워크 간에 통신을 하려면 라우터가 필요하다.
- 랜 안에서는 MAC 주소만으로도 통신할 수 있지만 네트워크 간에 통신을 하려면 IP 주소가 필요하다.
- 경로를 선택하고 목적지 IP 주소까지 어떻게 데이터를 전달할지 결정하는 것을 라우팅이라고 한다.
- 라우터의 라우팅 테이블에는 경로 정보가 등록되어 있다.
- 네트워크 계층의 대표적인 프로토콜에는 IP가 있다.