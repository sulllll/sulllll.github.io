---
layout: single
title:  " DAY-02. 자바 출력"
categories: Java
tag: [JAVA, 환경설정, 출력(print), 변수]
toc: true
toc_sticky: true
author_profile: true
sidebar:
  nav: "docs"
---
# 📌2022-02-24


## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## **1️⃣** 자바 환경 설정

- Eclipse protable EE사용
- Eclipse protable EE파일 압축 해제 후, 환경 설정 시작 → 숨긴파일 해제 후 eclipse.ini 파일에서 vm 부분을 설치한 jdk 파일의 위치로 변경
- Eclipse 실행 → file → new → project (반드시 프로젝트를 생성 해야한다)

## **2️⃣ 출력**

### 1. println : 한 줄씩 출력

### 2. print : 같은 줄에 출력

<script src="https://gist.github.com/kimyeong96/ef449e1412d8661ca2f481a6a8953227.js"></script>

출력

![1.png](/assets/images/posts/2022-02-24/1.png)


### “” 와 ‘’ 의 차이 (더블 vs 싱글)

<script src="https://gist.github.com/kimyeong96/097a9af18f1a44df374d336e12b15b95.js"></script>

- 자바에서 " " 와 ' ' 는 다르다
- 자바에서 " " : 문자열 , ““ 내용이 없어도 된다
- 자바에서 ‘ ‘ : 문자(한 글자만 가능) , ‘‘ 사이에 내용이 있어야 한다

### + : 문자열 연결 / 덧셈
<script src="https://gist.github.com/kimyeong96/da255e9ea444197b24141abb0ca121b7.js"></script>

![2.png](/assets/images/posts/2022-02-24/2.png)

### + : 문자열 + 숫자

<script src="https://gist.github.com/kimyeong96/9f3c832bef94ab9070c3e1f35b1802b8.js"></script>

- +는 왼쪽에서 오른쪽으로 더해짐
- 문자 + 숫자 = 문자

## 3️⃣ 변수

### 개념 정리

- 변수 : 메모리(RAM)에 값을 기록하기 위한 공간
- CPU :  사람의 뇌 , 기억은 못하고 처리(연산)만 한다
- RAM :  휘발성 메모리, CPU에서 처리한것을 기억
- HDD :  비휘발성 메모리
- Heap : new 연산자에 의해 동적으로 할당하고 저장되는 공간, 객체, 배열등
- Stack : 메소드를 호출하면 자동생성 메소드가 끝나면 자동소멸 지역변수, 매개변수 , 메소드 호출 스  택등

### 변수의 선언

❓ 메모리 공간에 데이터를 저장할 수 있는 공간을 항당하는 것

- 선언 방법 : 자료형 + 변수명 + ;
- 자료형

![3.png](/assets/images/posts/2022-02-24/3.png)

<script src="https://gist.github.com/kimyeong96/d2cc68c8c398f66f8fb5369e0abd5c14.js"></script>


변수명 짓기 ❗ 나쁜 예
<script src="https://gist.github.com/kimyeong96/60867380abd928c48e2339eedf8b6f52.js"></script>

