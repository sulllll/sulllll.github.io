---
layout: single
title:  " DAY-05. 자바 반복문 "
categories: JAVA-academy
tag: [JAVA, 반복문]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---
# 📌2022-03-02

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## **1️⃣ 반복문**

### 1. for

<script src="https://gist.github.com/kimyeong96/4a95cf8be3d55da56b53345bfd44413d.js"></script>


💡 Exam - 01 : 1부터 사용자가 입력한 값까지 출력한 코드를 작성

<script src="https://gist.github.com/kimyeong96/0ff7e045ae41794cfa3cb46c349f77e1.js"></script>

💡 Exam - 02 :  1부터 사용자가 입력한 값까지 홀수만 출력

<script src="https://gist.github.com/kimyeong96/66584771b7f81dd24a2cd172f43cbea4.js"></script>

- 방법2는 생각하지 못함

💡 Exam - 03 : Continue 이용

<script src="https://gist.github.com/kimyeong96/d6d3483f410d59ca0d0c525a52a2045c.js"></script>

- continue → 현재 진행되고 있는 반복 흐름이 종료

💡 Exam - 04 : 1부터 입력값까지의 전체 합을 출력

<script src="https://gist.github.com/kimyeong96/5975368447e59e2fd23613bb99fbb98a.js"></script>


- 지역변수 sum 확인
<details>
<summary>👈지역변수 </summary>
<div markdown="1">
반복문 / 조건문 혹은 메서드(기능)의 {} 안 범위에서만 사용할 수 있는 변수
</div>
</details>

### 2. while

<script src="https://gist.github.com/kimyeong96/d3a2d3f2ec4584c67b6c78ef99e7b18b.js"></script>

- for문과 같은 역할(반복) → 초기식 x ,
- 무한루프가 반복되는 상황일 때 사용
- while 문은 break문과 같이 쓰여야 한다