---
publish: true
permalink: logseq
created: 2023-11-27
updated: 
description: 
aliases:
  - Logseq
  - 로그시크
status: "[[Ongoing]]"
tags:
  - 📦Software
  - SecondBrain
---
Up:: 


### Plugin 추천
1. Tabs
2. Bullet Threading
3. Journals calendar
4. Awesome Links
5. Todo list
6. Image auto resizer
7. [[로그시크 - 스마트 블럭 플러그인 _ 템플릿 생성 버튼 만들기]]
8. swapblocks
9. Comment Block
10. TOC Generator

### Page Tips
#### 페이지 아이콘 만드는 방법
1. `::`을 입력하면 여러가지 옵션이 뜬다.
2. `icon`을 선택한다. 
3. 원하는 아이콘을 입력한다. 
4. Refresh를 하면 페이지 제목 앞에 아이콘이 바뀐다. 

#### Checkbox에 TODO 없애기
`custom.css`에 아래 코드를 삽입하면 됩니다. 
```css
.marker-switch.block-marker.TODO { 
display: none; 
}
```

`custom.css` 여는 방법: `Settings > General > Custom Theme > Edit custom.css`

Reference: 
- [(2) How to Insert a plain Checkbox? : logseq](https://www.reddit.com/r/logseq/comments/rw4hnx/how_to_insert_a_plain_checkbox/)

#### "Linked References" 항상 접기

1. `config.end`를 열어줍니다. 
   방법: `Settings > General > Custom Configuration > config.end`
2. 다음 줄을 찾습니다.  (`ctrl/cmd + F`로 검색하세요.)
   `ref/linked-references-collapsed-threshold`
3. 오른쪽의 숫자를 0으로 바꾸세요. 
   기본: `ref/linked-references-collapsed-threshold 50`
   **수정 후**: `ref/linked-references-collapsed-threshold 0`

#### "Linked References"의 블록 항상 접기(level 1만 보이게)
1. `config.end`를 열어줍니다. 
   방법: `Settings > General > Custom Configuration > config.end`
2. 다음 줄을 찾습니다.  (`ctrl/cmd + F`로 검색하세요.)
   `:ref/default-open-blocks-level`
3. 오른쪽의 숫자를 0으로 바꾸세요. 
   기본: `:ref/default-open-blocks-level 2`
   **수정 후**: `:ref/default-open-blocks-level 0`

 


Reference: [How to set Logseq to collapse "Linked References" by default, similar to "Unlinked References"? - Questions & Help - Logseq](https://discuss.logseq.com/t/how-to-set-logseq-to-collapse-linked-references-by-default-similar-to-unlinked-references/16127)

\
\
\
	

## Settings
##### Editor
- Preferred file format
- preferred date format
- Preferred workflow
- Show brackets
- Spell checker
- Logical outdenting
	- 동일한 수준의 불렛 A와 B가 줄줄이 있을 때, A를 outdent하면 A는 B의 아래로 이동합니다. 
	- 말 설명이 어렵죠?  `i` 라는 아이콘을 누르면 영상 설명을 볼 수 있으니 참고해주세요. 
