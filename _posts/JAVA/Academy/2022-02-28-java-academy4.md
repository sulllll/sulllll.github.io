---
layout: single
title:  " DAY-04. 자바 조건문"
categories: Java
tag: [JAVA, 조건문]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---
# 📌 2022-02-28


## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## **1️⃣  과제 코드 비교**

1) 내 코드

<script src="https://gist.github.com/kimyeong96/26ddb58552330a4cd972b0ecef98f78c.js"></script>


2) 강사님 코드
<script src="https://gist.github.com/kimyeong96/e5a16aab97e7de884218c2d81f44aaca.js"></script>

- 굳이 gender2를 다시 할당 할 필요없이 gender로 받아도 된다.

## **2️⃣ 조건문**

### 1. 기본 조건문

<script src="https://gist.github.com/kimyeong96/91d394f2c7eefb5edbaf478a1d2a24bb.js"></script>

- 조건식이 true이면 코드가 실행되고 false이면 코드가 실행되지 않는다.

### 2. else if / else

<script src="https://gist.github.com/kimyeong96/a83b268f47f37244bda198b21f0c5256.js"></script>

### 3. 간단한 퀴즈 1번

<script src="https://gist.github.com/kimyeong96/9deab45aebec48f11a25772146c8b9f8.js"></script>

### 4. 간단한 퀴즈 2번 : 조건문으로 만든 계산기

<script src="https://gist.github.com/kimyeong96/a732b8c0ad435bea6631e22fa19b6d13.js"></script>
- String은 " == " 이 아닌 equls() 로 비교한다

### 5. 심화 퀴즈 (중첩 if문)

<script src="https://gist.github.com/kimyeong96/9081ea2589badb9be0d732406d1988ff.js"></script>

### 6. switch / case

<script src="https://gist.github.com/kimyeong96/f856560a1e73ae682f47439609d7306b.js"></script>

- break가 없다면 아래와 같은 결과가 나온다 case가 사과 일때 실행되고 그 뒤에 코드도 실행이된다(파인애플)

    ![1.png](/assets/images/posts/2022-02-28/1.png)

- 뒤의 코드를 실행시키지 않기 위해서는 break; 를 해줘야한다
    - break를 만나는 순간 코드는 멈춘다

    ![2.png](/assets/images/posts/2022-02-28/2.png)

<script src="https://gist.github.com/kimyeong96/2f5ac8488ef3769938c7d7fb53d2de60.js"></script>
- 입력을 받아 해당하는 case의 코드 실행
- default는 if 조건문의 else역할