---
layout: post
title: "TIL(Today I learned)(190317)"
date: 2019-03-17
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


Java String.replaceAll 함수와 정규식

```
String str = "ab341A9k";
String lower = str.replaceAll("[^a-z]", "");
String upper = str.replaceAll("[^A-Z]", "");
String alphabets = str.replaceAll("[^a-zA-Z]", "");
String numbers = str.replaceAll("[^0-9]", "");

lower : "abk"
upper : "A";
alphabets : "abAk"
numbers : "3419"
```
