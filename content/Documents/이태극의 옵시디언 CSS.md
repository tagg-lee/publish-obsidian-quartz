---
permalink: obsidian-css-snippets-of-tagg
tags:
  - Topic
Keywords:
  - "[[Obsidian]]"
status: 
aliases: 
description: 
updated: 
publish: true
created: 2023-12-17
---


## Heaing 1~5 설정
```css
/* Reference */
/* 
1. https://forum.obsidian.md/t/heading-top-bottom-spacing-through-css/37424/3
2. https://forum.obsidian.md/t/remove-the-line-under-headings-custom-css/8620
*/

/* headings for editor and preview */

:root {
  --green: #036014; 
  --blue: #1f02b2;
  --orange: #FF4500;
  --purple: #430360;
  --red: #bd2000;
  --bold-color: var(--red);
}

i, em, span.cm-em {
color: var(--blue); 
}


/*********************************/
/* Section 1 for heading */
/*********************************/

.markdown-rendered h1,
.cm-s-obsidian .HyperMD-header.HyperMD-header-1{ 
  font-family: 'Times New Roman', serif !important;;
  font-weight: 500;
  font-size: 2em !important;
  color: black;
  padding-top: 50px;
  border-bottom: 0px !important;
}

.markdown-rendered h2,
.cm-s-obsidian .HyperMD-header.HyperMD-header-2 { 
  font-family: var(--font-family-editor);
  font-weight: 500;
  font-size: 1.8em !important;
  color: var(--green);
  padding-top: 10px;
  border-bottom: 2px solid #e0e0e0;
}

.markdown-rendered h3,
.cm-s-obsidian .HyperMD-header.HyperMD-header-3 { 
  font-family: var(--font-family-editor);
  font-weight: 500;
  font-size: 1.6em !important;
  color: var(--blue);
  padding-top: 10px;
}

.markdown-rendered h4,
.cm-s-obsidian .HyperMD-header.HyperMD-header-4 { 
  font-family: var(--font-family-editor);
  font-weight: 500;
  font-size: 1.4em !important; 
  color: var(--green);
}

.markdown-rendered h5,
.cm-s-obsidian .HyperMD-header.HyperMD-header-5 { 
  font-family: var(--font-family-editor);
  font-weight: 500;
  font-size: 1.2em !important; 
  color: var(--text-title-h5);
  padding: 14px 0 0px 0;
}


```