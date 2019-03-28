---
layout: post
title: "TIL(Today I learned)(190328)"
date: 2019-03-28
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

# 배포



### 롤링 업데이트

- 새 버전을 배포하면서, 새 버전 인스턴스를 하나씩 늘리고, 기존 버전을 하나씩 줄인다.
- 기존 버전과 새 버전이 동시에 존재할 수 있는 단점이 있지만, 시스템을 무장애로 업데이터할 수 있다.



### 카나리 배포

- 기존 버전을 유지한 채로 일부 버전만 신규 버전으로 올려 반응을 보고 배포



### 블루 그린 배포

- 블루, 그린 2개의 환경을 라우터로 전환하는 방식





# C++ 알고리즘

## memset

memset 함수는 어떤 메모리의 시작점부터 연속된 범위를 어떤 값으로(바이트 단위) 모두 지정하고 싶을 때 사용하는 함수이다.

```c++
void * memset ( void * ptr, int value, size_t num );
```

- ptr : 채우고자 하는 메모리의 시작 포인터(시작 주소)
- value : 메모리에 채우고자하는 값. int형이지만 내부에서는 unsigned char(1 byte)로 변환되어서 저장된다.
- num : 채우고자 하는 바이트의 수. 즉, 채우고자 하는 메모리의 크기


