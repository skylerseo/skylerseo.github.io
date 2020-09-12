---
title: JSX 란?
author: Skyler Seo
date: 2020-09-12 23:36:00 +0900
categories: [dev, react]
tags: [react, jsx]
---

```jsx
const element = <h1>Hello, world!</h1>;
```

위에 희한한 태그 문법은 문자열도, HTML도 아닙니다.

JSX라 하며 JavaScript를 확장한 문법입니다. UI가 어떻게 생겨야 하는지 설명하기 위해 React와 함께 사용할 것을 권장합니다. JSX라고 하면 템플릿 언어가 떠오를 수도 있지만, JavaScript의 모든 기능이 포함되어 있습니다.

JSX는 React “엘리먼트(element)” 를 생성합니다. 다음 섹션에서는 DOM에 어떻게 렌더링하는지 알아보겠습니다. 아래를 보면 JSX를 시작하기 위해 필요한 기본사항을 찾으실 수 있습니다.

# JSX란?

React에서는 이벤트가 처리되는 방식, 시간에 따라 state가 변하는 방식, 화면에 표시하기 위해 데이터가 준비되는 방식 등 렌더링 로직이 본질적으로 다른 UI 로직과 연결된다는 사실을 받아들입니다.

React는 별도의 파일에 마크업과 로직을 넣어 *기술*을 인위적으로 분리하는 대신, 둘 다 포함하는 “컴포넌트”라고 부르는 느슨하게 연결된 유닛으로 *[관심사*를 분리](https://en.wikipedia.org/wiki/Separation_of_concerns)합니다. 이후 섹션에서 다시 컴포넌트로 돌아오겠지만, JS에 마크업을 넣는 게 익숙해지지 않는다면 [이 이야기](https://www.youtube.com/watch?v=x7cQ3mrcKaY)가 확신을 줄 것입니다.

React는 JSX [사용이 필수가 아니지만](https://ko.reactjs.org/docs/react-without-jsx.html), 대부분의 사람은 JavaScript 코드 안에서 UI 관련 작업을 할 때 시각적으로 더 도움이 된다고 생각합니다. 또한 React가 더욱 도움이 되는 에러 및 경고 메시지를 표시할 수 있게 해줍니다.

# Materials

<https://ko.reactjs.org/docs/introducing-jsx.html>
<https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_getting_started>
