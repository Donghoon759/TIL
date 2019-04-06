---
layout: post
title: "TIL(Today I learned)(190404)"
date: 2019-04-04
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

## 서비스
- 포드는 컨트롤러에 의해 관리, 클러스터내를 옮겨다닌다.
- 노드를 옮기면서 실행되거나 클러스터내의 포드 IP가 변경되기도
- 동적으로 변하는 포드들에 접근하는 방법 -> 쿠버네티스의 서비스
- 포드가 어디에 있는지에 상관없이 고정된 주소를 이용해서 접근이 가능해진다.
- 클러스터 외부에서 포드에 접근하는것도 서비스를 통해 가능

## 서비스의 종류
- CluterIP : 기본 서비스 타입
	- 클러스터 내부에서 사용가능
	- 클러스터 내부의 노드나 포드에서 이 ClusterIP를 이용해 이 서비스에 연결된 포드에 접속 가능
	- 클러스터 외부에서는 이용불가
- NodePort : 각 노드의 지정된 포트를 할당하는 방식
	- 노드에 상관없이 포트번호만 서비스에 지정된걸 사용하면 접근가능
	- 클러스터 외부에서도 접근 가능
	- 클러스터외부에서 클러스터내부의 포드로 접근할 때 사용할 수 있는 가장 간단한 방법
- LoadBalancer : AWS, GCP 같은 클랄우드 서비스를 사용할때 사용가능한 옵션
	- 클라우드에서 제공해주는 로드밸런서와 포드를 연결해 그 로드밸런서의 IP를 이용해서 클러스터 외부에서 접근가능하게 해준다.
	- kubectl get service에서 EXTERNAL-IP 부분
- ExternalName : 서비스를 externalName의 값이랑 매치
	- 클러스터 내부에서 외부로 접근할때 주로 사용
	- 미리 설정해준 CNAME값으로 연결되서 클러스터 외부로 접근할 수 있음