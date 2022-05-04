---
layout: single
title:  "DAY-45 jquery event 활용"
categories: JAVASCRIPT
tag: [JAVASCRIPT, 자바스크립트, jquery event 활용]
toc: true
author_profile: false
sidebar:
  nav: "docs"

---

## 🚀 jquery event 활용

# 2022-05-03

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음




## 🔔 스크롤(화면) 이동

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="gOvpavK" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/gOvpavK">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


- 현재 스크롤의 위치를 알려면 (특정요소).prop("scrollHeight")를 줘야한다
- 스크롤의 위치를 변화시키려면 scrollTop()이라는 메서드를 사용해야 한다
- 화면이 위로 올라가기 위해서는 scrollTop()이 0이어야 하고 화면이 아래로 가기 위해선 scrollTop()이 현재 스크롤의 높이인 (특정요소).prop("scrollHeight")이어야 한다


## 🔔 엔터키 감지

- keyCode가 13이어야 한다
- 해당 글자의 keyCode를 아는 방법

```javascript
console.log(e.keyCode);
```


## 🔔 jquery effect
- slide down과 slide up을 사용해야 수직으로 변경된다
- hide와 show를 사용하면 구석으로 변경

- animation함수를 이용할 수 있다


### slide down / slide up 예제


1️⃣


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="BaYNzNr" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/BaYNzNr">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

- slideDown() -> display none 속성을 display block 으로 변경
- slideUp() -> display none으로 변경

2️⃣


<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="XWZbXze" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/XWZbXze">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>


### hide / show / toggle 예제
<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="eYVNzmw" data-user="kimyeong96" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/kimyeong96/pen/eYVNzmw">
  Untitled</a> by kimyeong96 (<a href="https://codepen.io/kimyeong96">@kimyeong96</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>