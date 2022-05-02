---
layout: single
title:  "DAY-43 정규표현식 활용"
categories: JAVASCRIPT
tag: [JAVASCRIPT, 자바스크립트, 정규표현식 활용]
toc: true
author_profile: false
sidebar:
  nav: "docs"
---

## 🚀 정규표현식 활용

# 2022-05-02

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음


## 자바스크립트에서의 정규 표현식

1. /패턴/ 사용 : ex)  let regex = /패턴/;
2. RegExp 생성자 사용 : ex)  let regex = new RegExp();

Example)


```javascript
let sample = "sky snew snow snows smile snowman snooze snows snuws snowly";

// snows의 문자패턴을 찾고 싶음
let regex1 = /snows/g;
let regex2 = new RegExp(/snows/g);
```


### 💡RegExp 함수

1️⃣ test(대상 문자열)

대상 문자열을 기준으로 패턴식에 일치하는 문자열이 있으면 true 없으면 false 반환, 포인터 개념(O)

```javascript
let sample = "sky snew snow snows smile snowman snooze snows snuws snowly";

let regex1 = /snows/g;
let regex2 = new RegExp(/snows/g);

// test를 사용하기 위해선 global 플래그를 붙여야한다
rs = regex1.test(sample);
console.log(rs); // true 첫번째 snows
rs = regex1.test(sample);
console.log(rs); // true 두번째 snows
rs = regex1.test(sample);
console.log(rs); // false 세번째 snows는 없기 때문에
```



2️⃣ exec(대상 문자열)

대상 문자열을 기준으로 패턴식에 일치하는 문자열을 찾아 배열로 반환, 몾찾으면 null 반환, 포인터 개념(O)

```javascript

sample = "심상 달구지 겨울 도롱뇽 가을 여름 막내 사과 파랑 심수봉 달무리";

let regex = /심상/g;

 // exec 역시 포인터의 개념이 있어 현재 가리키고 있는 값을 기억함

 rs = regex.exec(sample);
 console.log(rs); // index 25

 rs = regex.exec(sample);
 console.log(rs); // null

regex = /(심.+?)(달.{2})/g;
rs = regex.exec(sample);
console.log(rs); // 심상 달구지
// 0번 인덱스($&) 1번 인덱스($1) 2번 인덱스($2)
console.log(rs[0]); // &
console.log(rs[1]); // $1
console.log(RegExp.$1);
console.log(rs[2]); // $2
console.log(RegExp.$2);

console.log(rs[3]) //null

rs = regex.exec(sample);
console.log(rs) // 심수봉 달무리

일치하는 값 한번에 뽑기
while((rs = regex.exec(sample)) != null) {
console.log(RegExp.$1 +" : "+ RegExp.$2);
    // }
```


### 💡String 함수
1️⃣ 대상 문자열.match(패턴식)

일치하는 문자열의 배열을 반환해주는 함수 -> 일치하는 값이 없으면 null




``` javascript
sample = "심상 달구지 겨울 도롱뇽 가을 여름 막내 사과 파랑 심수봉 달무리";
regex = /(심.+?)(달.{2})/g;
rs = sample.match(regex);
console.log(rs); // ['심상 달구지', '심수봉 달무리']
```

2️⃣ 대상문자열.search(패턴식)

대상 문자열을 기준으로 패턴식에 일치하는 문자열의 인덱스를 반환, 못찾으면 -1 반환



```javascript
sample = "심상 달구지 겨울 도롱뇽 가을 여름 막내 사과 파랑 심수봉 달무리";
regex = /(심.+?)(달.{2})/g;

let rs = sample.search(regex);
console.log(rs); // 0 (일치하면 인덱스 값 반환)

rs = sample.search(regex);
console.log(rs); // 0 (일치하면 인덱스 값 반환)

```

3️⃣ replace


1) 문자열.replace(대상 값, 반환할 값) : 문자열에서 대상 값을 변환할 값으로 변환


```javascript
sample = "심상 달구지 겨울 도롱뇽 가을 여름 막내 사과 파랑 심수봉 달무리";
regex = /(심.+?)(달.{2})/g;

rs = sample.replace(regex, "none");
console.log(rs); // none 겨울 도롱뇽 가을 여름 막내 사과 파랑 none

let phone = '010-1234-1234';
regex = /-/g;
rs = phone.replace(regex, "");
console.log(rs); // 01012341234
```