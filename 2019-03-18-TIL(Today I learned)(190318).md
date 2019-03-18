---
layout: post
title: "TIL(Today I learned)(190318)"
date: 2019-03-18
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


## Pure ALOHA Protocol(unslotted)
무선 통신을 위한 Protocol이다. 각 station간 Synchronization을 하지 않고 전송 전 통신 Channel을 Listen하지 않는다. Multiple Access control Protocol이다.

1. Station이 전송할 frame이 생기면 바로 전송한다.
2. {max round trip time + a} 시간 동안 ACK를 기다린다.
3. ACK가 오면 성공, 그렇지 않으면 재전송한다.
4. Backoff limit에 이를 때까지 재전송이 반복되면, frame 전송을 포기한다.

## Slotted ALOHA Protocol
Pure ALOHA Protocol을 보완한 무선 통신 Protocol로, Carrier를 Sense하지 않는 점은 Pure ALOHA와 동일하지만, 각 station간 동기화 기법을 적용하여 ALOHA Network의 Throughput을 2배로 증가시켰다.

1. frame transmission time을 길이로 가지는 동일한 slot들을 인식하고 있는 station들은 central clock(또는 다른 동기화 mechanism)에 따라 slot의 시작 경계에서 전송을 시작한다.

2. fixed length frame의 전송시간과 일치하는 길이의 clock이 동기화 시스템에 의해 각 station에 적용되어 있고, 각 slot은 Success(S), Collision(C), Empty(E)의 3가지 state를 가진다.

3. 새롭게 전송할 frame이 생기면 다음 slot의 시작경계까지 기다린 후, 전송을 시작한다.

4. Collision은 2개 이상의 frame이 완전히 겹치는 slot에서 발생한다.