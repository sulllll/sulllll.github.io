---
layout: single
title:  " DAY-14. 자바 ArrayList"
categories: Java
tag: [JAVA, ArrayList]
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "docs"
---

# 📌2022-03-21

## 자바

<!--Quote-->

> ❗ 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## 1️⃣ 다형성

- 다양한 형태의 성질을 가지는 것
- 한 클래스가 다양한 클래스의 성질을 가질 수 있는 것
- 상속관계에서 부모타입의 참조변수가 자식타입의 인스턴스를 담을 수 있는 것

<script src="https://gist.github.com/kimyeong96/c619093128218a8bc081dbccb8694f1c.js"></script>

## 2️⃣ abstract / 추상클래스 / 추상메서드

- 추상메서드 : 메서드의 몸통을 만들지 않고 틀만 만들어 놓은 메서드 → 반드시 자식 메서드에서 재정의하여 사용해야하는 메서드
- 추상메서드를 하나라도 가진 클래스는 반드시 추상 클래스가 되어야한다
- 추상클래스 -> 더이상 직접 new를 못함

## 3️⃣ ArrayList : 똑똑한 동적 배열

<script src="https://gist.github.com/kimyeong96/2d1abc1d48c4450ee89e37273ad84cdd.js"></script>

### 메서드

1. add : 값 추가 (팬케익 쌓이는거 처럼 추가)
- list.add(2) →  정수 2를 리스트에 추가 , `list.add(new Integer(2)); 와 같다.`
- list.add(1,”A”) → 1번 인덱스에 “A”를 추가 → 기존의 1번 인덱스는 2번으로 밀림

1. remove : 값 삭제
- list.remove(2) → 2번 인덱스를 삭제해라
- list.remove(new Integer(2)) → 정수 2를 삭제해라

1. Collections.sort() : 오름차순으로 정렬
- Collections.sort(list);

1. size : 배열의 길이
- list.size(); → 들어가있는 데이터만큼만 자동으로 계산해서 배열길이를 알려준다

1. get : 해당 인덱스의 값 출력
- list.get(1) → list에서 인덱스가 1인 부분의 값을 구하기

1. subList : 원하는 인덱스의 값을 복사
- ArrayList list2 = new ArrayList(list.subList(2,4)); → 인덱스 2번 부터 3번까지 복사한 배열이 list2에 저 장

<script src="https://gist.github.com/kimyeong96/92c7d7b138f9f6317b65522fee8d411e.js"></script>

- ArrayList에서 charAt을 사용하려면 String으로 형변환 해준다음에 사용해야 한다
- ArrayList의 조상은 Object이다