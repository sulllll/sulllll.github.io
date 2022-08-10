---
layout: single
title:  " DAY-09. 자바 메서드,오버로딩"
categories: JAVA-academy
tag: [JAVA,  메서드, 오버로딩]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-08

## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## **1️⃣ 메서드(Method)**

<script src="https://gist.github.com/kimyeong96/6dd90f1a1f3470704a2e5fd6996cc3fc.js"></script>

- 메서드란, 어떤 특정한 작업을 수행하기 위해서 모아놓은 명령문의 집합 => function(함수)
- 정의부 : 메서드를 정의하는 영역 / 어떤 기능을 수행하게 될지에 대한 코드가 들어가는 영역
- 호출부 : 정의된 메서드 호출하는 영역 -> 즉 이미 정의된 메서드를 호출해서 그 기능을 쓰겠다 선언하는 영역
- 매개변수의 자료형과 인자값을 자료형과 수는 반드시 일치 해야함
- return 할게 없으면 반환자료형은 void
- 매개변수 인자값은 반드시 있어야 하는게 아님 -> 필수 x

### 1. Quiz-1 : 입력받은 만큼 출력

<script src="https://gist.github.com/kimyeong96/fcb8f33f50a4ec67f5680ed5c14d21da.js"></script>

### 2. Quiz-2 : 사용자가 입력한 채소를 영어 단어로 바꿔서 반환

<script src="https://gist.github.com/kimyeong96/a85e24392256fa37ed457db6dc80716f.js"></script>

## **2️⃣ 오버로딩(Overloading)**

<script src="https://gist.github.com/kimyeong96/7adc7cf477261045b0e6ed8ee6dece5e.js"></script>

- 메서드명은 같지만 매개변수의 개수가 다름
- 메서드명은 같지만 매개변수의 자료형이 다름
- 매개변수의 개수 or 자료형 or 둘 다 다르다면 오버로딩 성립

### 오버로딩 성립 x

<script src="https://gist.github.com/kimyeong96/71d39c43a15c52e29de92783ec238434.js"></script>

![1.png](/assets/images/posts/2022-03-08/1.png)

- 반환타입이 A와 B코드의 차이는 int에서 void로 다르다
- C 코드 : 리턴 자료형이 달라지고 + 매개변수의 형태 달라지게 되면 다른 메서드로써 같은 이름을 사용하는게 가능 → 오버로딩 X

