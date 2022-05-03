---
layout: single
title:  "DAY-44 jquery 시작"
categories: JAVASCRIPT
tag: [JAVASCRIPT, 자바스크립트, jquery]
toc: true
author_profile: false
sidebar:
  nav: "docs"

---

## 🚀 jquery 시작

# 2022-05-03

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음

## 🔔jquery 이용

- jquery cdn을 import 해와야 한다


## 🔔getElementsByClassName

- 배열 형태로 반환된다.




1️⃣ 자바스크립트 이용
<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="PoQwRze" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/PoQwRze">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


## 🔔jquery의 css / event 이용


### css
<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="VwQYXKz" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/VwQYXKz">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



### event
- jquery 이벤트 : on(이벤트명, 콜백함수)


1️⃣


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="VwQYXaW" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/VwQYXaW">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



- 자바스크립트의 innerHTML은 제이쿼리의 html()과 같다



2️⃣


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="NWyPYxE" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/NWyPYxE">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



- div이긴 한데 클래스명에 Div가 포함되는 div [출처](https://ggmouse.tistory.com/457)






3️⃣


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="YzePawx" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/YzePawx">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



- 자바스크립트의 value는 jquery의 val()과 같다



## 🔔선택자


### 자식 선택


1️⃣


자식 선택 -> 대상요소.children() :

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="yLvyKLr" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/yLvyKLr">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


💡 자식중 p 태그만 선택


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="zYRxWxG" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/zYRxWxG">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


2️⃣ 대상요소.find(선택자)


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="OJQPvPZ" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/OJQPvPZ">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>



- eq(n) : n번째 인덱스를 뽑기 위해 사용


### 부모 선택

- 대상요소.parent() : 대상 요소를 기준으로 부모 요소를 선택
- 대상요소.parents() : 대상 요소를 기준으로 모든 상위 요소를 선택

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="LYQEdVb" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/LYQEdVb">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


###  형제 선택



1️⃣ 내 부모의 형제 선택
```javascript
console.log($("h1").parent().next()); // container's 형제 This is span2
```



2️⃣ 형제 선택

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="qBxEoBN" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/qBxEoBN">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>




3️⃣ next, nextAll

- 특정요소.next() : 특정요소의 다음 엘레먼트 가져오기(하나)
- 특정요소.nextAll(선택자) : 특정요소의 다음의 모든 엘레먼트 가져오기(배열로 반환)


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="mdXyxbB" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/mdXyxbB">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>




4️⃣ prev, prevAll

- 대상요소.prev() : 대상요소를 기준으로 이전(앞)에 위치한 형제요소 선택
- 대상요소.prevAll(선택자) : 대상요소를 기준으로 이전(앞)에 위치한 모든 형제요소 선택

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="MWQYQMd" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/MWQYQMd">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


[정보](https://webzz.tistory.com/50)


5️⃣ first, last
- 대상요소.first() : 같은 태그 중에 가장 먼저 나온 엘레먼트 선택
- 대상요소.last() : 같은 태그 중에 가장 늦게 나온 엘레먼트 선택




<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="QWQwQeJ" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/QWQwQeJ">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


## 🔔jquery와 javascript의 차이

- jquery의 $(document).ready(function(){}는 javascript의 window.onload()와 같다

### 기존 요소에 값 넣어주기 (append / prepend)
<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="PoQwQvE" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/PoQwQvE">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>






### 기존 요소에 값 넣어주기 (before / after)

- before() : 동위관계에 있어 요소의 앞쪽에다가 요소를 추가
- after() : 동위관계에 있어 요소의 뒤쪽에다가 요소를 추가


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="yLvyvzx" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/yLvyvzx">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>