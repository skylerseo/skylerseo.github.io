---
title: 재귀함수(재귀호출함수)
author: Skyler Seo
date: 2020-09-09 02:57:00 +0900
categories: [dev, javascript]
tags: [javascript, recusive-function, function]
---

재귀 함수(Recusive function)는 자기 자신을 호출하는 함수를 말한다.

재귀 함수는 자신을 무한히 연쇄 호출하므로 호출을 멈출 수 있는 탈출 조건을 반드시 만들어야 한다.

탈출 조건이 없는 경우, 함수가 무한 호출되어 stackoverflow 에러가 발생한다.

대부분의 재귀 함수는 for나 while 문으로 구현이 가능하다.

반복문보다 재귀 함수를 통해 보다 직관적으로 이해하기 쉬운 구현이 가능한 경우에만 한정적으로 적용하는 것이 바람직하다.

```jsx
function loop(x) {
  if (x >= 10) return;
  loop(x + 1);
}

//Using ECMAScript 2015 arrow notation
const loop = (x) => {
  if (x >= 10) return;
  loop(x + 1);
};
```

```jsx
// 1부터 n까지 더하는 함수
function add(num) {
  if (num === 1) return 1;

  return num + add(num - 1);
}

console.log(add(9));
```

```jsx
// 피보나치 수열
// 피보나치 수는 0과 1로 시작하며, 다음 피보나치 수는 바로 앞의 두 피보나치 수의 합이 된다.
// 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, ...
function fibonacci(n) {
  if (n < 2) return n;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

console.log(fibonacci(0)); // 0
console.log(fibonacci(1)); // 1
console.log(fibonacci(2)); // 1
console.log(fibonacci(3)); // 2
console.log(fibonacci(4)); // 3
console.log(fibonacci(5)); // 5
console.log(fibonacci(6)); // 8
```

```jsx
// 팩토리얼
// 팩토리얼(계승)은 1부터 자신까지의 모든 양의 정수의 곱이다.
// n! = 1 * 2 * ... * (n-1) * n
function factorial(n) {
  if (n < 2) return 1;
  return factorial(n - 1) * n;
}

console.log(factorial(0)); // 1
console.log(factorial(1)); // 1
console.log(factorial(2)); // 2
console.log(factorial(3)); // 6
console.log(factorial(4)); // 24
console.log(factorial(5)); // 120
console.log(factorial(6)); // 720
```

## Materials

<https://developer.mozilla.org/ko/docs/Glossary/Function>
<https://poiemaweb.com/js-function#73-%EC%9E%AC%EA%B7%80-%ED%95%A8%EC%88%98>
