---
layout: post
title:  "Utternaces를 사용하여 블로그에 댓글 기능 추가하기"
date:   2023-11-06 17:02:29 +0900
categories: sample
published: true
---

## 첫번째, [Utterances](https://utteranc.es) 설치하기
[Utternaces](https://utteranc.es)에 접속해서 Install 버튼을 눌러 Utterances를 설치해줍니다.
<br/><br/><br/><br/>

## 두번째, 접근 허용할 repo 선택하기

<img src="/images/utterances repo.png">
<br/>
<p align= "center">모든 repo에 접근 가능하게 할 것인지, 원하는 repo에만 접근 가능하게 할 것인지 선택할 수 있습니다. 원하는 repo에만 접근할 수 있도록 하려면 Select repositories를 눌러 원하는 repo를 선택한 후 Save 버튼을 눌러 저장해줍니다.
<br/><br/><br/><br/>

## 세번째, 설정 페이지에서 저장소 설정하기
<img src="/images/utterances 1.png">
<br/>
<p align= "center">repo에 [사용자명/repo이름]을 입력해줍니다.
<br/><br/><br/><br/>

<img src="/images/utterances 2.png">
<br/>
<p align= "center">다음은 블로그 게시글의 경로를 설정하는 항목입니다.<br/>
저는 블로그 게시글의 경로를 이슈의 제목으로 설정했습니다.
<br/><br/><br/><br/>

<img src="/images/theme.png">
<p align= "center"> 원하는 댓글 기능 창 테마를 골라줍니다.
<br/><br/><br/><br/>

## 네번째, 적용을 위해 _layout/post.html에 추가하기
<img src="/images/code.png">
<br/>
<p align= "center"> 코드를 복사합니다.
<br/><br/><br/><br/>

<img src="/images/ju.png">
<br/>
<p align= "center"> 각자 사용하는 테마마다 disqus를 사용하는 것도 있고, 사용하지 않는 테마도 있는데 만약 disqus를 사용한다면 주석처리를 해줍니다. 저는 disqus를 사용하진 않지만, 기존에 있던 코드들을 모두 주석처리해주었습니다.
<br/><br/><br/><br/>

<img src="/images/add code.png">
<br/>
<p align= "center">아까 복사했던 Utterances 스크립트를 추가합니다.<br/>
변경 사항을 커밋한 후 Github 저장소에 push 합니다.

## 다섯번째, 확인해보기
<img src="/images/comment.png">
<br/>
<p align= "center">Github page에 들어가보면 댓글 기능이 추가된 것을 볼 수 있습니다.



