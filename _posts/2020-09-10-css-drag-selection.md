---
title: ::selection (마우스로 드래그(선택)했을 때)
author: Skyler Seo
date: 2020-09-10 07:23:00 +0900
categories: [dev, css]
tags: [css, selection, mouse, drag]
---

드래그 영역의 스타일을 바꾸고 싶은 경우 ::selection을 쓰면 된다.

```css
/* 문법 예시 */
.style ::selection {
  color: white;
  background: red;
  cursor: pointer;
  outline: none;
}
```

적용 가능 속성들은 아래와 같이 제한되어 있다.

- 텍스트 색상 - color
- 백그라운드 - background
- 커서의 종류 - cursor
- 외곽선 - outline
