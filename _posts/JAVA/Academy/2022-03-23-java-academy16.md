---
layout: single
title:  " DAY-16. 자바 IO스트림 심화"
categories: Java
tag: [JAVA, IO스트림]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-23

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


# 2022-03-23

## 1️⃣ 텍스트 파일 읽기

<script src="https://gist.github.com/kimyeong96/b151c17e34a3964b35fea7332003dde7.js"></script>

- **fis.close()를 사용하기 위해서는 try~catch를 반복해야 하기 때문에 try문 안에다가 FileInputStream fis = new FileInputStream("test.txt")를 써준다 → try~with~resource 구문**

### 1) 반복문을 활용해 읽기

<script src="https://gist.github.com/kimyeong96/b323d3442192d77501057d1d84660f16.js"></script>

- **FileInputStream은 byte자료형을 활용 → 배열을 활용**
- **아스키코드에서 32는 띄어쓰기, 엔터는 13**

### 2) 텍스트 파일 복사 퀴즈

<script src="https://gist.github.com/kimyeong96/c73187a9c53cdc3a8a0a2a18d9483451.js"></script>

### 3) FileReader / BufferedReader

<script src="https://gist.github.com/kimyeong96/308af9765c8d75631c9b24eb98dfdcc8.js"></script>