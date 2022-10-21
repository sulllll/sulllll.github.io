---
layout: single
title:  "DAY-41 배열,객체"
categories: Javascript
tag: [JAVASCRIPT, 자바스크립트, 배열,객체]
toc: true
author_profile: true
sidebar:
  nav: "docs"
---

## 🚀 Event 이용

# 2022-04-28

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## 🔔 indexOf

- 배열의 인덱스 위치를 반환해준다


<script src="https://gist.github.com/kimyeong96/22af8e8a57500e74cf9ca0d19c3a886d.js"></script>

## 🔔 concat

- 값이나 배열을 합칠 때 사용하는 함수
- 원래의 배열에 영향 x


<script src="https://gist.github.com/kimyeong96/91dc166ae0d703e7b5d1951fd241c847.js"></script>

## 🔔 reverse

- 배열의 순서를 뒤짚어주는 함수
- 원래의 배열에 영향을 준다


<script src="https://gist.github.com/kimyeong96/dfb90b2f3e7d233ba2118318b15be632.js"></script>

## 🔔 sort

- 배열안의 데이터를 오름차순 정렬 / 내림차순 정렬해주는 함수
- 원래의 배열에 영향을 준다
- 숫자의 경우 제대로 정렬이 되지않는다 -> 함수를 이용해야한다

<script src="https://gist.github.com/kimyeong96/480960bdb46f0f6eed63bf54e19fb115.js"></script>


### 숫자 sort
- sort() 함수의 인자값으로 compareFunction를 넘겨줘 오름차순, 내림차순을 정확히 해줄 수 있음
  - compareFunction(a,b) : 0보다 작은 수 반환(음수) -> a를 b보다 낮은 인덱스로 정렬 -> 오름차순
  - compreFunction(a,b) : 0을 반환 -> a와 b의 인덱스를 변경 x
  - compareFunction(a,b) : 0보다 큰 수 반환 -> b를 a보다 낮은 인덱스로 정렬 -> 내림차순


<script src="https://gist.github.com/kimyeong96/4759b781c6d5996735ee39707fd6a87f.js"></script>

## 🔔 배열의 요소 추가,삭제,수정


### 추가, 삭제
1. push : 가장 끝에 추가
2. pop : 가장 끝 삭제
3. unshift(값) : 가장 첫 인덱스에 새로운 값 추가(인덱스가 뒤로 밀려남)
4. shift(값) : 가장 첫 인덱스 값 삭제


<script src="https://gist.github.com/kimyeong96/77925555f039a360d0731e6a95e971e5.js"></script>


5. slice : 배열의 데이터를 잘라내는 함수
- slice(인자1, 인자2) : 배열의 데이터를 잘라내는 함수
  - 인자 1 = 시작 인덱스, 시작 인덱스에서부터 데이터를 잘라서 자른 데이터를 배열로 만들어 반환
  - 인자 2 = 끝 인덱스, 시작 인덱스에서부터 데이터를 끝 인덱스 전까지 잘라서 배열로 반환 -> 끝 인덱스(인자2)가 없으면 배열의 끝 인덱스까지 잘라버림
- 원본 배열에 영향 x

<script src="https://gist.github.com/kimyeong96/6fb22d057bb993f910a862db55c57615.js"></script>


1. splice(index, 제거수, [추가값]) : 시작 인덱스를 기준으로 해서 원하는 개수만큼 데이터를 제거할 수 있음

- 원본 배열에 영향이 있음
- 세번째 인자인 새로운 값을 추가하는 것도 가능 시작 index : 해당 인덱스로부터 값을 제거하라
- (만약 index 값만 인자로 넘겨주면 해당 인덱스로부터 나머지 인덱스 데이터 모두 삭제);


<script src="https://gist.github.com/kimyeong96/d2f2ad41f11f7b52f512798da66ab2d4.js"></script>


## 🔔 window.onload()

<script src="https://gist.github.com/kimyeong96/046142389b408b9d71bd064eb05c3a49.js"></script>

- script를 body 태그 위에서 실행 하면 오류 발생 -> script가 실행될 당시에 아직 div가 없는 상태여서(cannot set properties of null)
  - 따라서 window.onload를 활용해 에러 해결


## 🔔 객체

객체 생성법
- property = 자바에서의 맴버필드
- key,value = 자바에서는 멤버필드명이 key 멤버필드에 셋팅된 값이 value


1️⃣ 객체 생성자

<script src="https://gist.github.com/kimyeong96/3ccb7df1c258b9030bb89c6dc3b76adb.js"></script>

2️⃣ 생성자 함수

<script src="https://gist.github.com/kimyeong96/5859b75b618b1a4f1a05ff51e55fe18f.js"></script>

1)생성자 내부에서 가능한 작업
<script src="https://gist.github.com/kimyeong96/b117b8d5607d51b233d91a02d70d54c4.js"></script>




3️⃣ 객체 리터럴

<script src="https://gist.github.com/kimyeong96/56f2a583171835512abae71a30a4f70d.js"></script>

1) 리터럴 방식으로 속성에 함수 값 넣기


<script src="https://gist.github.com/kimyeong96/2d0ec922bea57284f899c5deee523b68.js"></script>

## key, value 찾기 연습

<script src="https://gist.github.com/kimyeong96/ec755fedc631a99afcc6bdc5ca33e102.js"></script>

1) americano 출력 -> key값이 "" 일때 []로 묶는다


<script src="https://gist.github.com/kimyeong96/9c0373158333a2d706e262eabc53b3d2.js"></script>

[출처](https://poiemaweb.com/js-object)

2) salley의 번호

<script src="https://gist.github.com/kimyeong96/c80500bf305f6264880addc6bd3a437e.js"></script>


3) tom의 번호

<script src="https://gist.github.com/kimyeong96/590988445c86967f4c47c7dd75817fb6.js"></script>
