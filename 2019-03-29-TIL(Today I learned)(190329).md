---
layout: post
title: "TIL(Today I learned)(190329)"
date: 2019-03-29
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

# CSS
## 자식 셀렉터와 자손 셀렉터

```css
ul strong { color : dodgerblue; }
```

strong이 ul의 하위이기만 하면 스타일이 적용.

```css
div > strong { background : yellow; }
```

strong이 div 바로 아래 직계여야 스타일이 적용.

## CSS 태그의 우선순위(4가 제일 높음)

1. 브라우저 디폴트 스타일
2. 스타일 시트 파일에 선언된 스타일
3. `<style></style>` 태그에 선언된 스타일
4. style 속성에 선언된 스타일

## font 스타일
- 글자체는 font-family : Arial, Serif;
- Arial이 없으면 Serif가 적용되는 구조.
- font : font-style, font-weight, font-size, font-family