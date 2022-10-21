---
layout: single
title:  " DAY-06. 자바 반복문,라벨링 "
categories: Java
tag: [JAVA, 반복문 탈출, labelling]
toc: true
toc_sticky: true
author_profile: true
sidebar:
  nav: "docs"
---

# 📌 2022-03-03

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## **1️⃣ 반복문 탈출**

## 1) break 2번 쓰기

<script src="https://gist.github.com/kimyeong96/3e1b35ed67e5fa30691e1bd36e6268fb.js"></script>

- switch 문안에서 break; 사용 switch 문 밖에서 break 사용 해야 10을 눌렀을때 반복문 탈출

## 2) labeling
<script src="https://gist.github.com/kimyeong96/01ffdf97fb1a9416d86467d9e410b81a.js"></script>

- while 문 앞에 원하는 이름의 라벨링을 붙여준다
- break문 뒤에 라벨링의 이름을 붙여준다.

## **2️⃣ 랜덤 함수 (Random)**

<script src="https://gist.github.com/kimyeong96/2aec512a65f241964aa004e5568977c2.js"></script>

- Math.random() : 0.0 ~ 1.0 사이의 난수를 생성

### 랜덤 Quiz

1. 오류

<script src="https://gist.github.com/kimyeong96/034b6ad1324cb69b0d0ea04a7f7202e3.js"></script>

![1.png](/assets/images/posts/2022-03-03/1.png)

- if 문에서 충족 안되고, else if 에서도 충족이 안되면 String에는 공간 만 할당이 되어있지 데이터가 담기지 않아 있다 그래서 오류가 발생

1. 오류 해결법

1)

<script src="https://gist.github.com/kimyeong96/0fe2912f79ab691afb023d597da83e3b.js"></script>

- String rs에 null값을 넣어 놓는다
- 그 후 조건문이 실행되면 null값 에서 “짝” 이나 “홀” 로 데이터가 바뀐다

2)

<script src="https://gist.github.com/kimyeong96/3382b51fc6a14a122a810ba8ccae6335.js"></script>

- String rs를 할당만 해둔다
- 조건문을 if / else if 가 아닌 if / else로  한다
- if / else if 는 if가 아니면 다른 else if를 보고 거기서도 아니면 또 다른 else나 else if를 필요로 한다.
- 반면 if / else는 if가 아니면 무조건 else의 코드가 실행이 된다. 그래서 if / else를 쓴다.

