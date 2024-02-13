---
aliases: 
created: 2023-10-22
tags: 
---



# 
Obsidian의 커뮤니티 플러그인 Dataview를 설명하는 문서입니다.

### Dataview 학습 방법
- [Basic Dataview Query Builder](https://s-blu.github.io/basic-dataview-query-builder/)
- [옵시디언 데이터뷰 Dataview 한 영상으로 완전정복! - YouTube](https://www.youtube.com/watch?v=r1_Ho8XfRMc) | [[브라이언]]
### Dataview Query Examples
>[!note] created today
>\```dataview
List FROM "" 
WHERE file.cday = date("옵시디언 플러그인  Tasks Documentation") 
SORT file.ctime asc
>\```

>[!note] last touched today
>\```dataview
List FROM "" 
WHERE file.mday = date("옵시디언 플러그인  Tasks Documentation") 
SORT file.mtime asc
>\```
