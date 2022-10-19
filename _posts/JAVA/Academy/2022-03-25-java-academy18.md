---
layout: single
title:  " DAY-18. 자바 네트워크 심화"
categories: Java
tag: [JAVA, 네트워크 연습]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-25

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## 1️⃣ readAllBytes

- 실제 파일의 데이터의 크기를 배열로 바이트 배열로 받기

### 1) Server

<script src="https://gist.github.com/kimyeong96/346db4cf489680951d57d96bafa5dc22.js"></script>

### 2) Client

<script src="https://gist.github.com/kimyeong96/f86a5fda536632feea8b8223093b1d4f.js"></script>

## 2️⃣ listFiles

- 디렉토리의 파일목록(디렉토리 포함)을 File배열로 반환한다.

> File[] files = file.listFiles() 와 같이 사용


### 1) Server
<script src="https://gist.github.com/kimyeong96/6f2fa31d412230e735ba5e367aa5226f.js"></script>

### 2) Client

<script src="https://gist.github.com/kimyeong96/f1e9e3708ca75a90665c15e7eabc82d6.js"></script>

- writeInt로 보내면 readInt로 받아줘야 한다

