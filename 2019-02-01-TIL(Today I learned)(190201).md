---
layout: post
title: "TIL(Today I learned)(190201)"
date: 2019-02-01
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---


- Local에서 Jekyll을 작업하는 법을 배웠다.
    - 호스팅한 상태에서 test를 하면 불필요한 commit들이 너무 많아서 지저분해보였다.
    - 내 블로그의 테마를 만든 사람이 알려준 방법대로 local환경을 구성했다.
    - 환경 세팅과정에서 몇몇 오류를 맞닥뜨렸지만(역시나) 구글링하면서 해결했다.(설치과정상 문제들)
    - 포스팅해보려고 했으나 내가 루비를 자세히 아는 것도 아니고 universe한 방법은 아닌 것 같아서 나중에 확실히 알게 되었을때 포스팅하기로!

- Local에서 작업을 하니 행복하다.
    - _config.yml를 건드리면 서버를 껐다켜야 반영되지만 그 외 다른 파일들을 수정했을때는 auto-regeneration기능이 활성화되어있어서 바로 반영된다.

- permalink에 대해서 공부했다.
    - 처음에는 permalink에 대해 잘 몰라서 임의로 설정했는데 지금은 확실히 알 수 있다.
    - Jekyll 공식문서가 공부하기에 명확하다.

- markdown 파일에 image 업로드 방법을 배웠다.
    - image를 assets폴더에 넣고 경로를 설정해서 업로드 하는 방법을 다른 형식으로 여러번 시도해봤지만 자꾸 404 error가 뜬다.(몇시간동안 이것만 했다.)
    - 그래서 github의 issue를 사용해서 링크를 따오는 방식으로 업로드하려고 한다.

[깃허브 README.md 파일에 이미지 업로드 하기](https://hanee24.github.io/2017/12/21/how-to-upload-image-with-github-readme)