---
layout: single
title:  " DAY-11. 자바 객체 배열"
categories: Java
tag: [JAVA, 객체, 객체 배열, char]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-11

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음

## **1️⃣ 객체 배열**

<script src="https://gist.github.com/kimyeong96/386bc41ff4cb429b6e33c5cf4231c52c.js"></script>

### 객체 배열의 형태

<script src="https://gist.github.com/kimyeong96/7db349f32e2ce605d99fb69d3d80d48e.js"></script>

![1.jpg](/assets/images/posts/2022-03-11/1.jpg)

- new를 만나면 Heap에 저장
<script src="https://gist.github.com/kimyeong96/60bde8e427ad16d4a8989d98efe432ca.js"></script>

### 수정

<script src="https://gist.github.com/kimyeong96/7ad9a18aacc869b0b9192ea48dd93a44.js"></script>

## **2️⃣ java.lang.Error: Unresolved compilation problem 오류 발생**

> 패키지에 빨간 불이 들어옴


![3.png](/assets/images/posts/2022-03-11/3.png)

![4.png](/assets/images/posts/2022-03-11/4.png)

1. 패키지를 클릭 후, Refresh 선택
2. Project 선택 후, Clean
3. 실행 후 변함없으면 이클립스 껐다 켜보기

- char Scanner 받기 : char ch = sc.nextLine().chatAt(0);