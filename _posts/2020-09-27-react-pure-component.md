---
title: React.PureComponent
author: Skyler Seo
date: 2020-09-27 13:52:00 +0900
categories: [dev, react]
tags: [react, pure-component, purecomponent]
---

`React.PureComponent`는 `React.Component`와 비슷합니다.

`React.Component`는 `shouldComponentUpdate()`를 구현하지 않지만, `React.PureComponent`는 props와 state를 이용한 **얕은 비교**를 구현한다는 차이점만이 존재합니다.

React 컴포넌트의 `render()` 함수가 동일한 props와 state에 대하여 동일한 결과를 렌더링한다면, `React.PureComponent`를 사용하여 경우에 따라 성능 향상을 누릴 수 있습니다.

# **주의**

`React.PureComponent`의 `shouldComponentUpdate()`는 컴포넌트에 대하여 얕은 비교만을 수행합니다. 따라서 컴포넌트에 복잡한 자료 구조가 포함되어있다면, 깊은 차이가 존재함에도 불구하고 차이가 없다고 판단하는 잘못된 결과를 만들어낼 수 있습니다. props와 state의 구조가 간단할 것으로 예상될 때에만 `PureComponent`를 상속하고, 깊은 자료 구조의 변화가 있다면 `[forceUpdate()](https://ko.reactjs.org/docs/react-component.html#forceupdate)`를 사용하세요. 또는 중첩된 데이터들을 빠르게 비교할 수 있도록 하려면 [불변 객체](https://facebook.github.io/immutable-js/)의 사용을 검토해보세요.

더 나아가 `React.PureComponent`의 `shouldComponentUpdate()`는 컴포넌트의 하위 트리에 대한 props 갱신 작업을 수행하지 않습니다. 자식 컴포넌트들이 “순수”한지 꼭 확인하기 바랍니다.


## Materials

<https://ko.reactjs.org/docs/react-api.html#reactpurecomponent>
