---
layout: single
title:  " DAY-08. 자바 배열"
categories: Java
tag: [JAVA, 배열]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-07

## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## **1️⃣** 오류 잡기

### 틀린코드

<script src="https://gist.github.com/kimyeong96/c181cd44eb6f97a5fb6850be12dd260c.js"></script>

- equals라는 메서드를 사용하기 위해서는 Character를 사용해야 한다.
- 반면 == 을 이용해서 사용하려면 원시형 타입인 char 이용

    ![1.png](/assets/images/posts/2022-03-07/1.png)

<details>
<summary>👈stackoverflow </summary>
<div markdown="1">
[https://stackoverflow.com/a/18781579](https://stackoverflow.com/a/18781579) 참조
</div>
</details>


### 옳바른 코드

<script src="https://gist.github.com/kimyeong96/4ad6b9b3f920f1626ec658790303ffc6.js"></script>

## **2️⃣** 배열(Array)

- 같은 자료형의 집합
- 같은 자료형 변수들을 모아서 하나의 이름으로 관리

<script src="https://gist.github.com/kimyeong96/69c49d5ace55940e4e1cf48dff359164.js"></script>

- int[] -> int형 배열을 의미(자료형)
- arr -> 변수명_ 참조변수
- new -> heap 영역에 저장 -> 배열은 참조자료형
- int[5] -> heap 영역에 5칸짜리 공간(변수)을 만들겠다


![2.jpg](/assets/images/posts/2022-03-07/2.jpg)


### Quiz-1

<script src="https://gist.github.com/kimyeong96/4de3ba4f5b24dcc35b9213e755ac3854.js"></script>

### Quiz-2

<script src="https://gist.github.com/kimyeong96/3b342a85da8eb0fa9caa6ca015258b90.js"></script>

### Quiz-3

<script src="https://gist.github.com/kimyeong96/d71f39629f114c416decef11b8de15a9.js"></script>

### for each

<script src="https://gist.github.com/kimyeong96/b9e5553c085beb443c0c3450a6440ce6.js"></script>

### 오류

<script src="https://gist.github.com/kimyeong96/80b007ebf40adb15a6a36f83dff29bf3.js"></script>

- int / Integer 주의

### try ~ catch

<script src="https://gist.github.com/kimyeong96/b0e81c9305219a65498297ea333cbe6b.js"></script>

![3.png](/assets/images/posts/2022-03-07/3.png)

<aside>
💡 수 입력을 하는 공간에 “가나다” 를 입력해서 에러 발생 → catch 안에 있는 코드 실행

</aside>

- try : 에러가 없을 때 코드 실행
- catch : try에서 에러가 발생했다면 코드 실행

### 🔨 배열의 수정

<script src="https://gist.github.com/kimyeong96/87fd46cf879339fbb7e39ca3cf2789e3.js"></script>

1. Quiz-1

<script src="https://gist.github.com/kimyeong96/f02da1805917d135f3e26bab38d156da.js"></script>

![4.png](/assets/images/posts/2022-03-07/4.png)

1. Quiz-2

<script src="https://gist.github.com/kimyeong96/46d6454637df47ae45f1d8f95ed39b48.js"></script>

- 방법2번 for문에서 조건식 hello.length/2 를 생각하지 못함


### 📙 배열의 복사

1. 얕은 복사

<script src="https://gist.github.com/kimyeong96/3e6d981f3572d582db2a99e4768f272a.js"></script>

![5.jpg](/assets/images/posts/2022-03-07/5.jpg)

- 같은 주소값을 가지는 공간을 가르키게 된다면 얕은 복사
- 한 참조 변수를 통해 값을 수정하면 다른 참조 변수의 주소값의 데이터도 수정된다.



1. 깊은 복사

<script src="https://gist.github.com/kimyeong96/eca540c574ef06ae3d3ce1ac375db45d.js"></script>

![6.jpg](/assets/images/posts/2022-03-07/6.jpg)

- 실제 배열 안에 들어있는 값만 복사가 이루어지는 것
- 원본 데이터에 영향을 미치지 않음


### 🧨배열의 삭제
<script src="https://gist.github.com/kimyeong96/1abc29199225e9671215fd686de515d0.js"></script>

1) Quiz-1
<script src="https://gist.github.com/kimyeong96/2a081b5709f8ee493f7d828f67216d16.js"></script>

- int 배열은 0으로 String 배열은 null로 삭제