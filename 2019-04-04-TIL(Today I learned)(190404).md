---
layout: post
title: "TIL(Today I learned)(190406)"
date: 2019-04-06
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

## DNS
- "foo" 라는 이름의 Service가 "bar"라는 namespace에 있다.
- "bar"에 있는 Pod은 "foo"에 대한 DNS query를 사용하면서 service를 쉽게 찾을 수 있다.
- "quux"라는 namespace의 Pod은 이 서비스를 "foo.bar"라는 쿼리로 찾는다.
- Normal(not headless) Service는
```[서비스명].[namespace명].svc.cluster.local```
형식의 DNS를 할당받는다.
- Pod은 hostname, subdomain이라는 optional한 property를 가진다.
- Pod이 my-host라는 hostname과 subdomain이라는 subdomain을 가지면 Domain name은 "my-host.subdomain.namespace.svc.cluster.local"이 된다.

### DNS의 존재를 깨닫는데 상당한 시간이 소요되었다.

### DNS를 사용하여 Service를 거친 Pod간의 통신에 성공했다.