---
layout: single
title:  " DAY-15. 자바 제네릭,IO스트림"
categories: JAVA-academy
tag: [JAVA, 제네릭, IO스트림]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-22

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


# 2022-03-22

## 1️⃣ 제네릭(Generic)

> ArrayList에 저장할 자료를 명시해주는 것

<script src="https://gist.github.com/kimyeong96/c51a2bd9b06c62d28f5c43031ffa86b9.js"></script>

- 제네릭 사용을 하면 String으로 명시를 미리 하기에 형변환없이 charAt 사용 가능

## 2️⃣ Wrapper Class

<script src="https://gist.github.com/kimyeong96/fcafebffebc209c7693e629e4f6a759e.js"></script>

- 기본 자료형들을 감싸고 있는 클래스 -> 기본 자료형을 마치 클래스처럼 사용하는게 가능하도록 해줌
- char와 int 는 Character와 Integer를 사용해야 한다

## 3️⃣ 예외 처리

<script src="https://gist.github.com/kimyeong96/ab3cb80c5c91c0276c675481f25a46ff.js"></script>

- **e.printStackTrace() : 에러의 발생근원지를 찾아서 단계별로 에러를 출력**
- **e.getMessage() : 에러의 원인을 간단하게 출력**
- **e.toString() : 에러의 Exception 내용과 원인을 출력**

### e.printStackTrace()

![1.png](/assets/images/posts/2022-03-22/1.png)

## 4️⃣ 코드 리뷰

### Netflix 프로그램 DAO 코드 비교 해보기

### 1) 내 코드

<script src="https://gist.github.com/kimyeong96/3f31e7894c6c5c8b2b5d8f4830eb2243.js"></script>

- 제네릭을 사용해서 타입을 Membership으로 고정해서 ((Membership)list.get(i)).getId().equals(id)) 처럼 쓸필요가 없이 list.get(i)).getId().equals(id) 같이 표현
- 반환타입도 void가 아닌 Membership과 ArrayList<Membership> 등으로 사용
- 특히 값 보여주기 에서 void가 아닌 반환타입을 ArrayList<Membership> 하고 return 으로 list로 주는거에서 차이를 보임
- 강사님은 메서드를 void로 거의 두지 않음

## 5️⃣ IO 스트림

<script src="https://gist.github.com/kimyeong96/4844284427c1ca620bee5681a0a66e07.js"></script>

- Checked Exception : 코드가 실제 실행되기도 전에 에러가 발생할 수 있다고 보여지는 에러 -> try catch 필
