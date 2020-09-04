---
title: JS에서의 배열은 객체이다
author: Skyler Seo
date: 2020-09-05 00:51:00 +0900
categories: [dev, javascript]
tags: [javascript]
---

# JS에서의 배열

```jsx
//JS에서의 배열은 객체이다
const numArr = [1, 2, 3, 4];
console.log(typeof numArr); //object
```

```jsx
//JS에서는 배열의 길이와 배열의 요소 개수가 같은 말일까? NO!
//초기화해주지 않은 요소는 empty라는 요소로 채워진다
const arr = [];
arr[2] = 3;

console.log(arr.length); //3
console.log(arr); //[ <2 empty items>, 3 ]
```

```jsx
//배열에 요소 추가하기
const numArr = [1, 2, 3, 4];

//배열을 직접 건드리는 방식 .push(추가요소)
numArr.push(5, 6);
console.log(numArr); //[ 1, 2, 3, 4, 5, 6 ]

//배열을 직접 건드리지 않는 방식 .concat(추가요소)
const result = numArr.concat(7, 8);
console.log(numArr); //[ 1, 2, 3, 4, 5, 6 ]
console.log(result); //[1, 2, 3, 4, 5, 6, 7, 8]
```

```jsx
//배열 속 요소 빼내기 .pop()
const numArr = [1, 2, 3, 4];

numArr.pop();
console.log(numArr); //[ 1, 2, 3 ]

numArr.pop();
console.log(numArr); //[ 1, 2 ]
```

```jsx
//배열 속 요소 순회하기
const nameArr = ['짱구', '철수', '영희', '맹구', '훈이'];

//1번째 방법
for (var i = 0; i < nameArr.length; i++) {
  console.log(`내 이름은 ${nameArr[i]}야`);
}
//2번째 방법
nameArr.forEach(function (name) {
  console.log(`내 이름은 ${name}야`);
});
//2번째의 ES6. 이렇게 쓰도록 하자!
nameArr.forEach((name) => console.log(`내 이름은 ${name}야`));

//내 이름은 짱구야
//내 이름은 철수야
//내 이름은 영희야
//내 이름은 맹구야
//내 이름은 훈이야
```

```jsx
//map
const oddArr = [1, 3, 5, 7, 9];

const result = oddArr.forEach((num) => num * 2);
console.log(result); //undefined

const mapResult = oddArr.map((num) => num * 2);
console.log(mapResult); //[ 2, 6, 10, 14, 18 ]

//map은 새로운 배열을 만들어준다는 점에서 forEach와 다르다.
//웬만하면 map을 쓰자
```

```jsx
//내가 원하는 조건을 만족하는 배열 속 요소 찾기
//filter()
const oddArr = [1, 3, 5, 7, 9];

const filterArr = oddArr.filter((x) => x > 4);
console.log(filterArr); //[ 5, 7, 9 ]

const postList = [
  { date: 'yesterday', id: 1 },
  { date: 'yesterday', id: 2 },
  { date: 'today', id: 3 },
  { date: 'today', id: 4 },
];

const todayPost = postList.filter((post) => post.date === 'today');
console.log(todayPost);
//[ { date: 'today', id: 3 }, { date: 'today', id: 4 } ]
```
