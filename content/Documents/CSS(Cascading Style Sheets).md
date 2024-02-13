---
permalink: cascading-style-sheets
tags:
  - 📦Software
Keywords:
  - "[[소프트웨어 개발(Software Development)]]"
status: 
aliases: 
description: 
updated: 
publish: true
created: 2023-12-17
---

## CSS란?
HTML의 디자인을 더 예쁘게 만들어주는 문법입니다. 

"HTML과 CSS는 프로그래밍 언어인가?"라는 질문에는 논란이 있습니다. 
어떤 개발자 부류는 프로그래밍 언어가 아닌 마크업(Markup) 언어라는 주장을 합니다.  예를들어 Markdown은 마크업 언어 중 하나입니다. 
## Questions

### 붙여쓰기, 띄어쓰기, `,`의 차이

제목을 영어로 표현하면 순서대로 다음과 같습니다:
1. Combining Selectors (without space)
   `.AAA.BBB`
2. Descendant Selector (with space)
   `.AAA .BBB`
3. Comma (Grouping Selector)
   `.AAA, .BBB`


위 3 가지는 서로 다른 기능을 합니다. 어떻게 사용하는지 예시를 통해 배워봅시다.
```html
<div class="aaa.bb">
  <div class="bbb"> combining selector (no space) </div>
</div>


<div class="aaa">
  <div class="bbb">descendant selector (space)</div>
</div>


<div class="aaa"> comma (grouping selector)</div>
<div class="bbb"> comma (grouping selector)</div>
```

```css
/* Combining Selectors (without space): */
.aaa.bbb {
  background-color: lightblue;
}


/* Descendant Selector (with space): */
.aaa .bbb {
  color: red;
}


/* Comma (Grouping Selector): */
.aaa, .bbb {
  font-weight: bold;
}
```