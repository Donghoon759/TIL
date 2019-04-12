---
layout: post
title: "TIL(Today I learned)(190411)"
date: 2019-04-11
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

## Scheduling mechanisms

- 네트워크 계층에서는 캡슐화할 때 IP 헤더를 추가한다.
    - scheduling : choose next packet to send on link
    - FIFO(First in First out) : send in order of arrival to queue
        - real world example?
        - discard policy : if packet arrives to full queue : who to discard?
            - tail drop : drop arriving packet
            - priority : drop/remove on priority basis
            - random : drop/remove randomly

    ## Scheduling policies : priority

    - send highest priority queued packet
    - multiple classes, with different priorities
        - class may depend on marking or other header info,
        - e.g. IP source/dest, port numbers, etc.

    → 우선순위 낮은애는 starvation

    ## Scheduling policies : Round Robin (RR) scheduling

    - multiple classes
    - cyclically scan class queues, sending one complete packet from each class (if available)

    ## Scheduling policies : Weighted Fair Queuing (WFQ)

    - generalized Round Robin
    - each class gets weighted amount of service in each cycle
    - 구현하기 힘들어서 변형들이 많다. (트래픽 플로우 간을 차별화 할 수 있는 메커니즘 구현이 어렵다.)
    - Fairness를 생각한 방법.
    - 1비트씩 보내는 것이 공정하지만 거의 불가능 → 1packet씩
    - 각 traffic flow로부터 오는 service 양을 고려해 Queuing displine도 적절히 맞춘다.
    - 각 Queue의 traffic 상황을 고려하여 바쁜 Queue에 capacity를 더 준다. 그렇다고 덜 바쁜 쪽을 닫는 것은 아님.
    - 혼잡제어를 위한 큐잉 메커니즘의 하나
        - 소량의 트래픽이 대량의 트래픽에 의해 손해를 보지 않도록 패킷 플로(Flow) 별로 서로 다른 큐를 두어 트래픽을 조절하고 (공정성)
        - 특정 기준에 따라 가중치를 정하여 같은 양의 트래픽을 가진 패킷 플로 간에서도 차별을 두는 방식 (가중치)
        - 

    ## The Internet network layer

    - host, router, network layer functions:

    [](https://www.notion.so/b81bcf886b6b4084bfe13bb8145cf458#c7c5da6cdee54236a59fa9428d56e8a5)

    - Transport layter : TCP, UDP (데이터 주고 받을 때 형식, 방법 등을 약속)
    - forwarding table은 일종의 routing table
    - network layer에서 event가 발생하면 physical layer로 내려옴

    ## IP datagram format