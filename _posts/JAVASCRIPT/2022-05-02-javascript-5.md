---
layout: single
title:  "DAY-43 정규표현식 활용"
categories: Javascript
tag: [JAVASCRIPT, 자바스크립트, 정규표현식 활용]
toc: true
author_profile: true
sidebar:
  nav: "docs"

---

## 🚀 정규표현식 활용

# 2022-05-02

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## 자바스크립트에서의 정규 표현식

1. /패턴/ 사용 : ex)  let regex = /패턴/;
2. RegExp 생성자 사용 : ex)  let regex = new RegExp();

Example)


<script src="https://gist.github.com/kimyeong96/8e9fbbf250469d56493268eb7f5edcb6.js"></script>


### 💡RegExp 함수

1️⃣ test(대상 문자열)

대상 문자열을 기준으로 패턴식에 일치하는 문자열이 있으면 true 없으면 false 반환, 포인터 개념(O)

<script src="https://gist.github.com/kimyeong96/47df3d833cff6c3d90f5ca02f4a32325.js"></script>



2️⃣ exec(대상 문자열)

대상 문자열을 기준으로 패턴식에 일치하는 문자열을 찾아 배열로 반환, 몾찾으면 null 반환, 포인터 개념(O)

<script src="https://gist.github.com/kimyeong96/ada15aea12568395bc3d74ef5bd99593.js"></script>


### 💡String 함수
1️⃣ 대상 문자열.match(패턴식)

일치하는 문자열의 배열을 반환해주는 함수 -> 일치하는 값이 없으면 null


<script src="https://gist.github.com/kimyeong96/a985a1eab5e286794866c957d6b22b52.js"></script>

2️⃣ 대상문자열.search(패턴식)

대상 문자열을 기준으로 패턴식에 일치하는 문자열의 인덱스를 반환, 못찾으면 -1 반환


<script src="https://gist.github.com/kimyeong96/9137d463b75d1a6e47a19592427ec07e.js"></script>

3️⃣ replace


1) 문자열.replace(대상 값, 반환할 값) : 문자열에서 대상 값을 변환할 값으로 변환


<script src="https://gist.github.com/kimyeong96/91540dc81bc4a868b36ca01e32f7f7f5.js"></script>


### 정규표현식 정보
1. [블로그](https://chrisjune-13837.medium.com/%EC%A0%95%EA%B7%9C%EC%8B%9D-%ED%8A%9C%ED%86%A0%EB%A6%AC%EC%96%BC-%EC%98%88%EC%A0%9C%EB%A5%BC-%ED%86%B5%ED%95%9C-cheatsheet-%EB%B2%88%EC%97%AD-61c3099cdca8)
2. [공식사이트](https://ko.javascript.info/regexp-introduction)