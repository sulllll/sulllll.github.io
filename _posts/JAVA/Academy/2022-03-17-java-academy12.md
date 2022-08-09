---
layout: single
title:  " DAY-12. 자바 상속"
categories: JAVA-academy
tag: [JAVA, 상속, super]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-17

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## 1️⃣ toString 오버라이딩

<script src="https://gist.github.com/kimyeong96/ce63c4ed09af1239d8ad2da9af63bd46.js"></script>

- toString으로 오버라이딩 되서 std와 std.toString과 같다

## 2️⃣ 메서드 주의 사항

- 메서드 내에서는 출력문을 작성하지 않는다

## 3️⃣ Object

![1.png](/assets/images/posts/2022-03-17/1.png)

- 모든 자료형의 최고 조상
- 회색부분의 글씨가 의미하는 것 : 메서드가 존재하는 클래스의 이름을 보여준다 ex) setName은 Product라는 클래스 안에 존재한다

## 4️⃣ 상속

부모

<script src="https://gist.github.com/kimyeong96/0cd039ce75cfa4ac374a3bae5b4b0632.js"></script>

자식

<script src="https://gist.github.com/kimyeong96/887ffc12a7ca7360b03e51fb4438d225.js"></script>

- super()를 통해 iceCream형 생성자를 호출하면 부모 클래스의 인스턴스 또한 생성된다.
- 부모클래스의 기본생성자를 호출하는 작업이다
- super()는 코드의 가장 첫 줄에 와야한다

## 5️⃣ 오버라이딩

부모
<script src="https://gist.github.com/kimyeong96/e230dae33c0e820000deec9f2b44d91a.js"></script>

자식

<script src="https://gist.github.com/kimyeong96/177a470f58965df391fef755cb39d922.js"></script>

- 부모클래스가 가지고 있는 메서드를 재정의하는 작업
- 똑같은 이름의 메서드, 똑같은 반환타입, 똑같은 매개변수
- 오버라이딩된 메서드가 (부모보다) 우선 실행
- 부모의 price는 private이기 때문에 getPrice()로 값 가져오기
- 여기서 오버로딩은 똑같은 이름의 메서드를 매개변수 자료형이나 개수를 달리해주는 작업