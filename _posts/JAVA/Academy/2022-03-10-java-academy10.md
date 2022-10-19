---
layout: single
title:  " DAY-10. 자바 객체"
categories: Java
tag: [JAVA, 객체, 라이브러리]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-10

## 자바
<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## **1️⃣ 과제 코드 리뷰**

- 메서드 내에서 System.out.println을 해주는 것이 아닌 메서드의 타입을 Void가 아닌 String으로 한뒤 return으로 돌려주기

## **2️⃣ 클래스와 객체**

<script src="https://gist.github.com/kimyeong96/72787bb62c19c7c619c301313dd1c9bb.js"></script>

- 패키지명은 소문자로 작성
- Laptop을 특성과 기능으로 나뉘어서 생각 → 특성은 맴버 변수 , 기능은 맴버 메서드



Laptop 클래스를 실행하는 파일

<script src="https://gist.github.com/kimyeong96/764d8e7158c80236c2096639ab76fa6a.js"></script>

<script src="https://gist.github.com/kimyeong96/005fa1cf1f377bf6d69163f1af32b635.js"></script>

![1.jpg](/assets/images/posts/2022-03-10/1.jpg)

![2.jpg](/assets/images/posts/2022-03-10/2.jpg)

- new는 Heap영역에 저장을 의미

### 특징

1. 추상화 : 노트북이 가지고 있는 특성, 기능을 추려내는 작업
2. 정보은닉(캡슐화) : 사용자가 접근하면 안되는 데이터들을 내부적으로 숨기거나 접근을 제한하는 것, 접근제한자 사용

### 접근 제한자

1. public : 외부, 모든 곳에서 접근이 가능
2. private : 반드시 해당 클래스 내부에서만 접근 가능
3. protected : 같은 패키지 혹은 상속
4. default : 같은 패키지 안에서는 모두 접근이 가능

## 3️⃣ getter / setter - 정보은닉
<script src="https://gist.github.com/kimyeong96/acdbe7a425aba7536fc251e35a29208a.js"></script>

- private으로 맴버변수를 설정하면 getter / setter 필수
- getter와 setter의 이름설정은 get + 맴버변수 이름 / set + 맴버변수 이름
- getter : read-only > setter : write-only(getter와 setter는 반드시 public 으로 해야한다)
- setter는 메서드이기에 조건을 둘수있다.
- 자동생성 방법 : 우측마우스 → source → Generate Getters and Setters

## 4️⃣ 생성자 (Constructor)

- 리턴타입 없음
- 클래스명과 이름이 같음
- 인스턴스가 만들어질 때 초기화 해주는 역할
- 기본생성자는 명시하지 않아도 알아서 생성해줌
- 다만 매개변수가 있는 생성자를 정의하는 순간부터는 기본생성자를 자동으로 만들어주지 않음
- 생성자 또한 메서드이기 때문에 오버로딩이 가능
- 자동생성 방법 : 우측마우스 → source → Generate Constructors using fileds

## 5️⃣ JOptionPane

### 1) showInputDialog

<script src="https://gist.github.com/kimyeong96/13a8238071be10b802d63effe3641a73.js"></script>

![3.png](/assets/images/posts/2022-03-10/3.png)

- JOptionPane.showInputDialog의 반환은 String으로 된다. → 정수나 다른 형으로 바꾸려면 Parse사용

### 2)showMessageDialog

```java
String name = JOptionPane.showInputDialog("1. 이름을 입력하세요."); //String으로 반환된다.
JOptionPane.showMessageDialog(null, name); // 첫번째는 null 값
// JOptionPane.showMessageDialog(null, args); // args는 String 뿐만 아니라 다른타입도 가능
```

- 이름을 톰이라고 입력했을 때의 결과

![4.png](/assets/images/posts/2022-03-10/4.png)

### 3) 예제 코드

<script src="https://gist.github.com/kimyeong96/67053f05374e2fb1aca005217e88bd5e.js"></script>

## 6️⃣ 라이브러리 사용

- 패키지 우측 마우스 build path 클릭 > java bulid path >  Libraries > Classpath > Add External jars
- try ~ catch 문에서 catch 안에 e.printStackTrace(); 사용