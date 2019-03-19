---
layout: post
title: "TIL(Today I learned)(190319)"
date: 2019-03-19
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


## Introduction to React
- React는 프레임워크가 아닌 라이브러리이다.
- React는 자바스크립트만 공부하면 쓸 수 있다.
- React는 model, view, controller 중 view이므로 Django, Ruby on Rails, Node.js와 섞어 쓸 수 있다.

### create-react-app package
어려운 webpack대신 react 코드를 손쉽게 자바스크립트 코드로 바꿔준다.
```
npm install -g create-react-app
```

### Component 정의
- React 앱을 만들기 전 만들어야 할 Components들을 정의한다.

- jsx는 리액트 컴포넌트를 만들때 사용하는 언어.(React로 작성하는 html)

- 모든 컴포넌트는 render function을 갖고 있다.

- ReactDom은 웹사이트에 출력(render)을 도와주는 모델

- Component => Render => Return => JSX

- React props, state

- this.props -> 데이터 참조

- list를 줄 때 key={index}도 줘야한다.

