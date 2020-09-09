---
title: SCSS @mixin 헬퍼
author: Skyler Seo
date: 2020-09-10 07:25:00 +0900
categories: [dev, css]
tags: [css, scss, sass, mixin, helper]
---

```scss
/// 내부 float을 해제하는 헬퍼
/// @author Nicolas Gallagher
/// @link http://nicolasgallagher.com/micro-clearfix-hack/ Micro Clearfix
@mixin clearfix {
  &::after {
    content: '';
    display: table;
    clear: both;
  }
}
```

```scss
/// 요소 크기를 설정하는 헬퍼
/// @author Hugo Giraudel
/// @param {Length} $width
/// @param {Length} $height
@mixin size($width, $height: $width) {
  width: $width;
  height: $height;
}
```

```scss
/// 벤더 프리픽스를 산출하는 믹스인 헬퍼
/// @access public
/// @author HugoGiraudel
/// @param {String} $property - 프리픽스가 붙지 않은 CSS 속성
/// @param {*} $value - 가공되지 않은 CSS 값
/// @param {List} $prefixes - 산출할 프리픽스 리스트
@mixin prefix($property, $value, $prefixes: ()) {
  @each $prefix in $prefixes {
    -#{$prefix}-#{$property}: $value;
  }

  #{$property}: $value;
}
```

---

```sass
// vendor prefix
@mixin vendorPrefix($property, $value) {
  @each $prefix in -webkit-, -moz-, -ms-, -o-, '' {
    #{$prefix}#{$property}: $value;
  }
}

.border_radius {
  @include vendorPrefix(transition, 0.5s);
}
```

```css
/* 위의 코드를 컴파일한 결과 */
.border_radius {
  -webkit-transition: 0.5s;
  -moz-transition: 0.5s;
  -ms-transition: 0.5s;
  -o-transition: 0.5s;
  transition: 0.5s;
}
```

---

```sass
// opacity
@mixin opacity($opacity) {
  opacity: $opacity; /* All modern browsers */
  $opacityIE: $opacity * 100;
  filter: alpha(opacity=$opacityIE); /* For IE5~IE9 */
}

.box {
  @include opacity(0.5);
}
```

```css
/* 위의 코드를 컴파일한 결과 */
.box {
  opacity: 0.5;
  /* All modern browsers */
  filter: alpha(opacity=50);
  /* For IE5~IE9 */
}
```

---

```sass
// position
@mixin position($position, $top: null, $right: null, $bottom: null, $left: null) {
  position: $position;
  top: $top;
  right: $right;
  bottom: $bottom;
  left: $left;
}

.box {
  @include position(absolute, $top: 10px, $left: 50%);
}
```

```css
/* 위의 코드를 컴파일한 결과 */
.box {
  position: absolute;
  top: 10px;
  left: 50%;
}
```

# Materials

<https://sass-guidelin.es/ko/#mixins>
