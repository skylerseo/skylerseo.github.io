---
title: CSS 선택자에 대한 모든 것
author: Skyler Seo
date: 2020-09-05 01:31:00 +0900
categories: [dev, css]
tags: [css, selector]
---

# All about CSS Selector

구체적으로 태그 가까이 다가가서 지정해주는 스타일의 우선순위가 더 높음

```css
/* naver로 시작하는 아이들만 골라서 색깔 바꿔줌 */
a[href^='naver'] {
  color: purple;
}

/* .com으로 끝나는 아이들만 골라서 색깔 바꿔줌 */
a[href$='.com'] {
  color: purple;
}

/* love를 포함한 아이들만 골라서 색깔 바꿔줌 */
a[href*='love'] {
  color: purple;
}

/* 다른 태그에 달려있는 special 아이디는 무시하고 li의 special만 변경 */
li #special {
  color: blue;
}

/* .apple이면서 .banana이기도 한 것 */
.apple.banana {
  color: red;
}
```

div selects all <div> elements.

p selects all <p> elements.

#cool selects any element with id="cool"

ul#long selects <ul id="long">

p strong selects all <strong> elements that are inside of any <p>

#fancy span selects any <span> elements that are inside of the element with id="fancy"

#cool span selects all <span> elements that are inside of elements with id="cool"

.neato selects all elements with class="neato"

ul.important selects all <ul> elements that have class="important"

#big.wide selects all elements with id="big" that also have class="wide"

p, .fun selects all <p> elements as well as all elements with class="fun"

a, p, div selects all <a>, <p> and <div> elements

p \* selects any element inside all <p> elements.

ul.fancy \* selects every element inside all <ul class="fancy"> elements.

p + .intro selects every element with class="intro" that directly follows a <p>

div + a selects every <a> element that directly follows a <div>

A ~ B selects all B that follow a A

A > B selects all B that are a direct children A

:first-child selects all first child elements.

p:first-child selects all first child <p> elements.

div p:first-child selects all first child <p> elements that are in a <div>.

span:only-child selects the <span> elements that are the only child of some other element.

ul li:only-child selects the only <li> element that are in a <ul>.

:last-child selects all last-child elements.

span:last-child selects all last-child <span> elements.

ul li:last-child selects the last <li> elements inside of any <ul>.

:nth-child(8) selects every element that is the 8th child of another element.

div p:nth-child(2) selects the second p in every div

:nth-last-child(2) selects all second-to-last child elements.

span:first-of-type selects the first <span> in any element.

div:nth-of-type(2) selects the second instance of a div.

.example:nth-of-type(odd) selects all odd instances of a the example class.

span:nth-of-type(6n+2) selects every 6th instance of a <span>, starting from (and including) the second instance.

p span:only-of-type selects a <span> within any <p> if it is the only <span> in there.

div:last-of-type selects the last <div> in every element.

p span:last-of-type selects the last <span> in every <p>.

div:empty selects all empty <div> elements.

:not(#fancy) selects all elements that do not have id="fancy".

div:not(:first-child) selects every <div> that is not a first child.

:not(.big, .medium) selects all elements that do not have class="big" or class="medium".

a[href] selects all <a> elements that have a href="anything" attribute.

[type] selects all elements that have a type="anything" attribute

[value] selects all elements that have a value="anything" attribute.

a[href] selects all <a> elements that have a href="anything" attribute.

input[disabled] selects all <input> elements with the disabled attribute

input[type="checkbox"] selects all checkbox input elements.

.toy[category^="Swim"] selects elements with class toy and either category="Swimwear" or category="Swimming".

img[src$=".jpg"] selects all images display a .jpg image.

img[src*="/thumbnails/"] selects all image elements that show images from the "thumbnails" folder.

[class*="heading"] selects all elements with "heading" in their class, like class="main-heading" and class="sub-heading"

Material site↓

[https://flukeout.github.io/](https://flukeout.github.io/)
