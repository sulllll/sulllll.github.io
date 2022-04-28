---
layout: single
title:  "DAY-39 배열,객체"
categories: JAVASCRIPT
tag: [JAVASCRIPT, 자바스크립트, 배열,객체]
toc: true
author_profile: false
sidebar:
  nav: "docs"
---

## 🚀 Event 이용

# 2022-04-26

<!--Quote-->
> ❗ 수업을 듣고, 개인이 공부한 내용을 적은 것 이기에 오류가 많을 수도 있음



## 🔔 indexOf

- 배열의 인덱스 위치를 반환해준다


```javascript
let tempArr = ['a','b','c','d'];
let index = tempArr.indexOf('a');
console.log(index); // 0 출력
```

## 🔔 concat

- 값이나 배열을 합칠 때 사용하는 함수
- 원래의 배열에 영향 x


```javascript
let arr1 = ['바나나','딸기','수박'];
let arr2 = ['사과','귤'];
let arr3 = [10,20,30];

let data1 = arr1.concat(arr2);
console.log(data1); // ['바나나', '딸기', '수박', '사과', '귤']

let data2 = arr1.concat("망고");
console.log(data2); // ['바나나', '딸기', '수박', '망고']

let data3 = arr1.concat(arr2,arr3);
console.log(data3); // ['바나나', '딸기', '수박', '사과', '귤', 10, 20, 30]

// concat은 원래의 배열에 영향 x
console.log(arr1); // ['바나나','딸기','수박'];
```

## 🔔 reverse

- 배열의 순서를 뒤짚어주는 함수
- 원래의 배열에 영향을 준다


```javascript

let arr1 = [1,2,3,4,5,6,7,8,9,10];
let arr2 = ['홍길동','임꺽정','세종대왕','이순신'];

arr1.reverse();
console.log(arr1); // [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

arr2.reverse();
console.log(arr2); // ['이순신', '세종대왕', '임꺽정', '홍길동']

```

## 🔔 sort

- 배열안의 데이터를 오름차순 정렬 / 내림차순 정렬해주는 함수
- 원래의 배열에 영향을 준다
- 숫자의 경우 제대로 정렬이 되지않는다 -> 함수를 이용해야한다

```javascript
let arr1 = ['마','가','다','아','하','나'];
let arr2 = [4,3,5,6,8,2,1,7,10];

arr1.sort();
console.log(arr1); // ['가', '나', '다', '마', '아', '하']


// 숫자의 경우 제대로 정렬이 되지 않는다
arr2.sort();
console.log(arr2); // [1, 10, 2, 3, 4, 5, 6, 7, 8] -> 문자로 인식해서 1이 먼저나오기에 1다음에 10이 나온다
```


### 숫자 sort
- sort() 함수의 인자값으로 compareFunction를 넘겨줘 오름차순, 내림차순을 정확히 해줄 수 있음
  - compareFunction(a,b) : 0보다 작은 수 반환(음수) -> a를 b보다 낮은 인덱스로 정렬 -> 오름차순
  - compreFunction(a,b) : 0을 반환 -> a와 b의 인덱스를 변경 x
  - compareFunction(a,b) : 0보다 큰 수 반환 -> b를 a보다 낮은 인덱스로 정렬 -> 내림차순


```javascript
function sortASC(a, b) {
  return a - b; // 오름차순
}

function sortDESC(a, b) {
  return b - a; // 내림차순
}

function sortStrDesc(a,b) { // 내림차순
  if(a > b) {
    return 1;
  }else if( b < a) {
    return -1;
  }else {
    return 0;
  }
}

arr2.sort(sortASC);
console.log(arr2); // [1, 2, 3, 4, 5, 6, 7, 8, 10]

arr2.sort(sortDESC);
console.log(arr2); // [10, 8, 7, 6, 5, 4, 3, 2, 1]

```

## 🔔 배열의 요소 추가,삭제,수정


### 추가, 삭제
1. push : 가장 끝에 추가
2. pop : 가장 끝 삭제
3. unshift(값) : 가장 첫 인덱스에 새로운 값 추가(인덱스가 뒤로 밀려남)
4. shift(값) : 가장 첫 인덱스 값 삭제


```javascript
fruits.push('strawberry');
console.log(fruits); // ['apple', 'banana', 'mango', 'strawberry']

fruits.pop();
console.log(fruits); // ['apple', 'banana', 'mango']

fruits.unshift('watermelon');
console.log(fruits);

fruits.shift('watermelon'); // ['watermelon', 'apple', 'banana', 'mango']
console.log(fruits); // ['apple', 'banana', 'mango']

```


1. slice : 배열의 데이터를 잘라내는 함수
- slice(인자1, 인자2) : 배열의 데이터를 잘라내는 함수
  - 인자 1 = 시작 인덱스, 시작 인덱스에서부터 데이터를 잘라서 자른 데이터를 배열로 만들어 반환
  - 인자 2 = 끝 인덱스, 시작 인덱스에서부터 데이터를 끝 인덱스 전까지 잘라서 배열로 반환 -> 끝 인덱스(인자2)가 없으면 배열의 끝 인덱스까지 잘라버림
- 원본 배열에 영향 x

```javascript
let data = ['apple','banana','mango','watermelon','grape'];
// 1번 인덱스 전까지만 삭제
console.log(data.slice(1)); //['banana', 'mango', 'watermelon', 'grape']

// 1번 인덱스 ~ 3번인덱스 앞까지 보여주기
console.log(data.slice(1,3)); // ['banana', 'mango']
console.log(data) //  ['apple', 'banana', 'mango', 'watermelon', 'grape']

```


2. splice(index, 제거수, [추가값]) : 시작 인덱스를 기준으로 해서 원하는 개수만큼 데이터를 제거할 수 있음

- 원본 배열에 영향이 있음
- 세번째 인자인 새로운 값을 추가하는 것도 가능 시작 index : 해당 인덱스로부터 값을 제거하라
- (만약 index 값만 인자로 넘겨주면 해당 인덱스로부터 나머지 인덱스 데이터 모두 삭제);


```javascript
let data2 = ['apple','banana','mango','watermelon','grape'];

// 인덱스 1번남 남기고 다 지움
data2.splice(1);
console.log(data2); // ['apple']

// 인덱스 1번 부터 1개를 지우고 그 자리에 strawberry를 넣어줌
data2.splice(1,1,"strawberry");
console.log(data2); // ['apple', 'strawberry', 'mango', 'watermelon', 'grape']

// 1번 인덱스 자리 부터 0개를 지우고 그 자리에 strawberry를 넣어준다 -> 즉 1번 인덱스에 strawberry 추가
data2.splice(1,0,'strawberry');
console.log(data2); // ['apple', 'strawberry', 'banana', 'mango', 'watermelon', 'grape']

data2.splice(-1);
console.log(data2); // ['apple', 'banana', 'mango', 'watermelon']
```


## 🔔 window.onload()

```html
<script>
let fruits = ['Apple','Orange','Tomato','Banana','Grape','StrawBerry'];

// window : 웹브라우저의 모든 요소를 담는 객체
// window.onload : 웹브라우저의 모든 요소들이 로드(준비)가 완료됐을때;

window.onload = function () {
  let list = document.getElementById('list');
  list.innerHTML = fruits;

  document.getElementById("btnUnshift").onclick = function () {
    let texUnshift = document.getElementById("texUnshift");
    fruits.unshift(texUnshift.value);
    list.innerHTML = fruits;
    texUnshift.value = "";
  }

  document.getElementById("btnshift").onclick = function() {
    fruits.shift();
    list.innerHTML = fruits;
  }

  document.getElementById("btnPush").onclick = function() {
    let texPush = document.getElementById("texPush");
    fruits.push(texPush.value);
    list.innerHTML = fruits;
    texPush.value = '';
  }

  document.getElementById('btnPop').onclick = function() {
    fruits.pop();
    list.innerHTML = fruits;
  }
}
</script>
```

- script를 body 태그 위에서 실행 하면 오류 발생 -> script가 실행될 당시에 아직 div가 없는 상태여서(cannot set properties of null)
  - 따라서 window.onload를 활용해 에러 해결


## 🔔 객체

객체 생성법
- property = 자바에서의 맴버필드
- key,value = 자바에서는 멤버필드명이 key 멤버필드에 셋팅된 값이 value


1️⃣ 객체 생성자

```javascript
 let member = new Object();
 console.log("전 : ", member); // {}

 member.id = "abc123";
 member.pw = "1234";
 console.log("후 : ", member) // {id: 'abc123', pw: '1234'}

 // key값의 중복 -> id 값이 변경
 member.id = "eee555";
 console.log("id 변경 후 ", member); // {id: 'eee555', pw: '1234'}

 // ket 값 출력
 console.log(member.id); // eee555
```

2️⃣ 생성자 함수

```javascript
// 2. 생성자 함수 -> 함수명 대문자
let Member = function(id,pw) {
this.id = id;
this.pw = pw;
}

let member2 = new Member("ab123",'55555');
console.log(member2); // Member {id: 'ab123', pw: '55555'}
```

1)생성자 내부에서 가능한 작업
```javascript
 let Member = function(id,pw) {
   this.id = id;
   this.pw = pw;
   let age = 20;
 }

 let member1 = new Member("abc123","1234");

 console.log(member1.id); // abc123
 console.log(member1["id"]); // abc123

 // 생성자 내부에서 선언한 일반 변수는 외부에서 접근 불가
 console.log(member1.age); // undefined;


 let Member = function(id,pw) {
   this.id = id;
   this.pw = pw;
   let age = 20;

   this.getAge = function() {
     console.log(age);
   }
 }

 let member1 = new Member("abc456", "4567");
 console.log(member1); // Member {id: 'abc456', pw: '4567', age: ƒ}
 console.log(member1.getAge); // ƒ () {console.log(age);}
 console.log(member1.getAge()); // undefined
 member1.getAge(); // 20
```




3️⃣ 객체 리터럴

```javascript

 let member = {
   id : 'abc123',
   pw : '1234',
 }

 console.log(member); // {id: 'abc123', pw: '1234'}

```
1) 리터럴 방식으로 속성에 함수 값 넣기


```javascript
let member = {
id : "abc123",
pw : "1234",
getAge : function() {
  console.log(20);
},
cart : ["Mango", "Apple"]
}

console.log(member.cart); // ['Mango', 'Apple']
console.log(member.cart[0]); // Mango

// 새로운 속성 추가 가능
member.nickname = '초콜렛';
console.log(member); // {id: 'abc123', pw: '1234', cart: Array(2), nickname: '초콜렛', getAge: ƒ}
```

## key, value 찾기 연습

```javascript
let cafe = {
 menu : {
   "drink-alcohol" : ["beer","soju"], // key 값이 여러개의 합성어이면 ""로 묶기
   "drink-coffee" : ['americano', 'latte'],
   desert : ['cake','cookie'],
 },

 employee : [
   function() {
     return {name : 'tom', phone : '010-5555-6666'}
   },
   {name : 'salley', phone : '010-1234-4567'}
 ]
}
```

1) americano 출력 -> key값이 "" 일때 []로 묶는다


```javascript
console.log(cafe.menu['drink-coffee'][0]);
```
[출처](https://poiemaweb.com/js-object)

2) salley의 번호


```javascript
console.log(cafe.employee[1].phone);
```


3) tom의 번호


```javascript
console.log(cafe.employee[0]().phone);
```


