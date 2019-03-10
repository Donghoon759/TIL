---
layout: post
title: "TIL(Today I learned)(190202)"
date: 2019-02-02
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title/
comments: true
tag: TIL
---


## Javascript로 Todo List 만들기
- 사용자에게 이름을 받아와서 localStorage에 저장하는 기능을 구현했다.(localStorage.setItem(currentUser, text);)
	- 페이지가 load되었을때 localStorage에 사용자 이름이 있으면 `Hello, 사용자이름!`을 출력하고 없으면 이름을 요청한다.
- Todo List기능을 구현했다.
	- submit event의 default기능을 껐다.(event.preventDefault();)
	- 왜냐하면 default기능은 text의 value를 빈칸으로 초기화해버리기 때문이다.
	- 그 후에 document.createElement 메소드를 통해서 li 태그를 넣고 그 밑에 DeleteButton과 text를 나타낼 span을 붙인다.
	- todo들은 여러개 이므로 생길때마다 빈 객체로 초기화한 배열에 넣어준다.
	- 그리고 이것도 localStorage에 저장하는데, 자바스크립트의 data를 localStorage에 저장할 수 없다고 한다.
	- 그래서 꼼수로 JSON.stringify() 메서드를 사용해서 Object->String으로 바꾸고 저장을 한다.
	- localStorage에 있는 Todo를 load할때는 JSON.parse() 메서드를 사용해서 String으로 저장해 놓았던 데이터를 다시 Object 형식으로 가져온다.

---