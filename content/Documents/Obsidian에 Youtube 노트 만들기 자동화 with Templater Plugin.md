---
permalink: obsidian-automation-with-templater-for-youtube-video
tags: 
Keywords: 
status: 
aliases: 
description:  
updated:
publish: true
created: 2023-12-24
---


## 템플렛
세컨드브레인 커뮤니티의 @꾸준히 님께서 만들어주신 템플렛입니다. 

```template
---
<%*
let url = await tp.system.clipboard();
url = url.replace(/app=desktop&|app=mobile&|m\./g, '');
let response = await fetch(`https://youtube.com/oembed?url=${url}&format=json`);
let data = await response.json();

let title = data.title.replaceAll(/[\/:*?"<>|]/g, '');
let author = data.author_name;
let author_url = data.author_url;
let html = data.html;
let thumbnail_url = data.thumbnail_url;

let newPath = "/500. Sources/2. Media/Utube/" + title;
await tp.file.move(newPath);
let regex = /v=(.*)/gm;
let m = regex.exec(url);

let newTitle = title;
let movedFile = app.vault.getAbstractFileByPath(newPath);
if (movedFile) {
    let content = await app.vault.read(movedFile);
    let frontmatterEnd = content.indexOf("---", 1);
    let frontmatter = content.substring(0, frontmatterEnd);
    let body = content.substring(frontmatterEnd);
    frontmatter = frontmatter.replace(/title: .*\n/, `title: ${newTitle}\n`);
    await app.vault.modify(movedFile, frontmatter + body);
}
-%>
title: <% title %>
tags:
  - video/utube
created: <% tp.file.creation_date("YYYY-MM-DD") %>
last modified: <% tp.file.last_modified_date("YYYY-MM-DD") %>
---
# <% title %>
* * *
> [!meta]+ Metadaten
> Source:: [<% title %>](<% url %>)
> Channel: [<% author %>](<% author_url %>)
> Published: 
> Watched: <% tp.date.now() %>

* * *
## Video Player
![player](<% url %>)
* * *
## Thumbnail
![Thumbnail](<% thumbnail_url %>)
* * *
## ScreenShot

* * *
## Transcript

* * *
## Note

* * *
## Thought

<% tp.file.cursor(0) %>
```