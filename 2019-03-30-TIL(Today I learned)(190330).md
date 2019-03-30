---
layout: post
title: "TIL(Today I learned)(190330)"
date: 2019-03-30
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

## 리액트 공부

### Mounting
React 컴포넌트의 인스턴스가 생성되고 DOM에 삽입되는 과정의 life cycle
- constructor
- componentWillMount
- render
- componentDidMount

<hr>

this.setState에서 ...this.state.movies과 추가할 State를 넣으면 기존 State를 유지한 채 update할 수 있다.

- 클래스 컴포넌트 : state있다.
- 함수형 컴포넌트 : state없다. props만있다. return만있음

