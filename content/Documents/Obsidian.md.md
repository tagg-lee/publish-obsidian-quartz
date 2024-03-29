---
title: 옵시디언(Obsidian)
permalink: 
tags:
  - 🏷️Document
  - 📦Software
Keywords: 
aliases: 
description: 
updated: 
created: 2024-02-26
publish: true
---
free-tags:: 
</br>
</br>

## What it is?
- [Obsidian](https://obsidian.md)은 지식관리를 위한 오픈소스 노트 앱 입니다. 
- 사용자들은 직접 Plugin을 개발하여 적용 수 있고, Community Plugin을 통해 유표할 수 있습니다. 



## Community Plugin 추천
- Front Matter Title
	- 파일 이름과 노트 제목을 다르게 사용할 경우에 유용하다. 



## 검색 (search)
### Search (Core plugin)
#### 옵션(Options)
- path
- file
- tag
- line
- selection
- [property]

#### 북마크하기
![](https://i.imgur.com/wSpwiCk.jpg)

1. 좌측 하단에 점 3개 있는 아이콘 클릭
2. `Bookmark...` 클릭
3. 값 지정 후 `Save` 클릭

### Bookmark (Core plugin)
#### 옵션(Option)
- Files
- Folders
- Graphs
- Searches
- Headings
- Blocks



To make it a little easier you could [bookmark](https://help.obsidian.md/Plugins/Bookmarks) the search with example text like `[permalink: EXAMPLE]`. Then you could just click the bookmark, double-click `EXAMPLE` to select it, type the permalink, and press Return.


## CSS snippet
#### 헤더 첫머리 요소에 `#` 기호를 보여주기
```CSS
h1::before {
  content: "# ";
  opacity:0.3;
}
h2::before {
  content: "## ";
  opacity:0.3;
}
h3::before {
  content: "### ";
  opacity:0.3;
}
h4::before {
  content: "#### ";
  opacity:0.3;
}
h5::before {
  content: "##### ";
  opacity:0.3;
}
h6::before {
  content: "###### ";
  opacity:0.3;
}
```

## 웹클리핑

웹클리핑은 크게 두 가지 유형이 있습니다.

1. 북마클렛이나 크롬 익스텐션
웹페이지를 마크다운 파일로 저장합니다. 

2. Sync to Read it later service 
Readwise, Omnivore 등의 서비스에 클리핑한 뒤 동기화 합니다. 
Read it later service는 웹클리핑 전용 서비스입니다. 그래서 옵시디언보다 편리한 점들이 있습니다. 

## 배터리 절약
Reference:
- https://forum.obsidian.md/t/battery-economy-when-taking-notes-syncing-on-tablet-laptop/47620/5

방법
- **Sync 끄기** (또는 주기 설정)
- 사용하지 않거나 배터리 소모가 큰 **플러그인 끄기**
	- (Core) Graph view
- 노트에 **GIF 사용하지 않기**