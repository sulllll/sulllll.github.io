---
layout: single
title:  " DAY-03. 자바 형변환,연산자,Scanner "
categories: Java
tag: [JAVA, String, 형변환, 연산자, Scanner]
toc: true
toc_sticky: true
author_profile: true
sidebar:
  nav: "docs"
---
# 📌2022-02-25


## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## **1️⃣ String : 참조형 변수**

![1.jpg](/assets/images/posts/2022-02-25/1.jpg)

- 기본형은 값이 저장 되지만, 참조형은 주소값이 저장된다

## **2️⃣ 형변환(Casting)**

- 데이터의 자료형을 변환
- 개발자가 데이터의 타입의 범위를 예측하지 못했을때
- 개발자가 원하는 대로 데이터 타입을 사용하기 위해서 강제적으로 형변환

### 형변환 종류

1. 자동 형변환(promotion) : 작은 자료형에서 큰 자료형으로 변환이 이루어지는 경우 ex) byte → int

<script src="https://gist.github.com/kimyeong96/dea769a86f2a91732336575c98f77989.js"></script>

1. 강제 형변환(down casting) : 큰 자료형에서 작은 자료형으로 변환이 이루어지는 경우 (데이터의 손실이 일어날 수 있음)

<script src="https://gist.github.com/kimyeong96/ffed71f2682e6df4e86ee8fd731af8f7.js"></script>

- 값의 범위가 큰 자료형을 값의 범위가 작은 자료형으로 변환
- 강제 형변환 시 데이터 손실 발생 → 데이터의 변형, 손실을 감수하고 변환
- 바꾸고 싶은 자료형을 ( ) 안에 기입
- 실수 → 정수  형변환 필요

### 형변환 Quiz

<script src="https://gist.github.com/kimyeong96/0607eaa4b800c31a49acfd80bd4158b0.js"></script>

## 3️⃣ 연산자(Operation)

1. 산술 연산자(+, -, *, /, %)
2. 대입 연산자(=, +=, -=, *=, /=, %=)
3. 비교 연산자(<, >, >=, <=, ==, !=)
4. 증감 연산자(전위 연산, 후위 연산)
5. 논리 연산자(&&, ||)
6. 삼항 연산자 ( 조건식? 식1 : 식2 )

### 산술 연산자

<script src="https://gist.github.com/kimyeong96/8dfaf4e45e6a72e4e5b7927e75f5ffd4.js"></script>

### 대입 연산자

<script src="https://gist.github.com/kimyeong96/962b0354216b2f74d77a94a09be1dad1.js"></script>

### 비교 연산자

<script src="https://gist.github.com/kimyeong96/e24f3532e046cfd0e80d15b8ebd090e5.js"></script>

- 참조 자료형 String 값에 대한 비교를 할 때는 ==을 쓰지 않고 equals()를 이용한다

### 증감 연산자

<script src="https://gist.github.com/kimyeong96/a15e48b383744ea8cc334a019270cf21.js"></script>

### 논리 연산자

<script src="https://gist.github.com/kimyeong96/c501e9ff4a54dd30ccbefcced9ef74d4.js"></script>
- true가 나오는 순간 바로 실행이 끝난다 ex) 첫 번째 연산에서 true면 두번째 연산은 실행 x

### 삼항 연산자

<script src="https://gist.github.com/kimyeong96/dda949cf0072aa4fe313501ea17e3e5f.js"></script>



## 4️⃣ Scanner

<script src="https://gist.github.com/kimyeong96/5a4d70db87d2cfd06b2bd478af8560de.js"></script>

- Scanner : 출력용으로만 쓰던 console 창에 입력도 가능하게 해주는 자바(jdk)에 내장된 도구
- Scanner를 사용하기 위해서 java.util.Scanner를 import 해줘야 한다
- next()는 한번에 여러개의 입력을 받을 수 없다. → 띄어쓰기, 엔터키 직전의 값만 받아준다
- nextLine()이여야 한번에 여러개의 입력을 받을 수 있다

![2.png](/assets/images/posts/2022-02-25/2.png)

### Scanner 연습
<script src="https://gist.github.com/kimyeong96/b62eb60304adfe866ef04b0470b9cb42.js"></script>

- 항목 하나하나 입력을 받을 때는 nextLine() 사용

### Scanner 연습2
<script src="https://gist.github.com/kimyeong96/72e9d4277b5e10c0d0b08e33e39dd74a.js"></script>




