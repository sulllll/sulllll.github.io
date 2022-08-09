---
layout: single
title:  "DAY-37 자바스크립트 시작"
categories: JAVASCRIPT
tag: [JAVASCRIPT, 자바스크립트]
toc: true
author_profile: false
sidebar:
  nav: "docs"
---

## 🚀 자바 스크립트 시작

# 2022-04-25

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## 🔔변수 선언

var : function level scope


let,const : block level scope



<script src="https://gist.github.com/kimyeong96/061927130fbc16194796d6f245d704f3.js"></script>

### scope

- function level scope : 하나의 함수 내에서 선언한 변수는 해당 함수 내에서 공유되는 경우
- block level scope : 하나의 블록 내에서 선언한 변수는 그 블록 내에서만 공유가 가능한 경우 (자바에서의 지역변수)

<script src="https://gist.github.com/kimyeong96/110315f22ceafebedd8fc265dd116eda.js"></script>

## 🔔type
자바스크립트에서의 자료형
- String, boolean, number, Bright, null, undefined, Symbol(고유한 값을 만들고자 할 때 사용하는 자료형)
  - undefined : 변수를 선언하고 그 변수에 값이 대입되지 않았을 경우
  - null : 값 자체가 없는 경우

<script src="https://gist.github.com/kimyeong96/3e3887274196847e918de5dff7e487bb.js"></script>


## 🔔basicFunction

### 알림창
1) alert

- 기본적인 알림창(확인 버튼 하나가 뜬다)


<script src="https://gist.github.com/kimyeong96/3d4eeba07a76e8b627d98498ce7e0c17.js"></script>


1) confirm

- 알림창(확인 버튼과 취소 버튼이 나옴)


<script src="https://gist.github.com/kimyeong96/48d2ff84d3fa9650385be5c3bfe78cd1.js"></script>


3) prompt

- 알림창(확인과 취소, 입력창을 띄워준다)
- 입력한 결과값을 return 해줌

<script src="https://gist.github.com/kimyeong96/9cf05c7adab070cea43f18d6e81a9d19.js"></script>

## 🔔selector

### getElementById
<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="PoEvRgj" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/PoEvRgj">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


1. value : input, textarea, select 태그들은 value를 통해서 값에 접근 가능
2. innerHTML : innerHTML을 통해 input, textarea, select 태그들을 제외하고 값에 접근 가능

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="RwxmyNp" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/RwxmyNp">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



## 🔔함수

- 자바스크립트에서 함수는 값처럼 사용가능

<script src="https://gist.github.com/kimyeong96/f509575425c90e26b286b1dea491f536.js"></script>

### 익명함수


- 이름이 없는 함수

<script src="https://gist.github.com/kimyeong96/66560a697509cfa436ec7e01cd133e40.js"></script>


## 이벤트

- 이벤트 : 브라우저 안에서 사용자가 취하는 모든 액션
(클릭, hover, drag, 스크롤, 크기조절..)

- call back function : 함수안의 파라미터로 다른 함수를 호출

- event listener(이벤트 감시자)
: 특정한 이벤트가 발생했을 때 그 이벤트를 감지하는 역할

- event handler(이벤트 처리자)
: 특정한 이벤트가 감지됐을 때 그에 따른 처리코드를 수행하는 역학

- e-> 일어난 이벤트에 대한 정보

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="jOYopmG" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/jOYopmG">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<script src="https://gist.github.com/kimyeong96/548ca0d8884efaf9ed5396f55d075188.js"></script>