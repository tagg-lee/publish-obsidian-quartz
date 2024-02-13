---
permalink: get_youtube-thumbnail
tags: 
Keywords: 
status: 
aliases: 
description:  
updated:
publish: true
created: 2023-10-13
---


## 이미지 URL을 쓰는 이유

이미지를 다운로드하면 내 컴퓨터나 서버의 용량을 차지한다.

하지만 URL을 사용하면 용량을 차지하지 않으면서 이미지를 사용할 수 있다.

다만, 영상을 올린 사람이 썸내일을 바꾸면 이미지가 함께 바뀐다는 문제점가 있긴하다.

하지만 내가 사용하는 용도에서는 그게 큰 문제가 되지 않기 때문에 그냥 쓰련다.

이미지 URL을 사용하는 팁을 하나 알려주자면, Imgur라는 서비스가 있으니 알아보길 바란다.

(언젠가 Obsidian과 Imgur을 연동하는 글을 쓰겠다.     )

## 방법

유튜브 영상의 링크를 보면 다음과 같은 형식일 것이다.

`https://www.youtube.com/watch?v=_ID_`

`_ID_` 이 부분은 그 영상의 고유한 ID이다. 그 ID 값만 복사한다.

그 다음 아래 URL의 `_ID_` 부분에 해당 영상의 ID를 입력한다. (둘 중에 하나를 골라서 쓰면 된다.)

그 URL이 바로 썸내일 이미지의 URL이 된다.

```
https://i.ytimg.com/vi/_ID_/hqdefault.jpg    // 표준 화질
https://i.ytimg.com/vi/_ID_/maxresdefault.jpg // 최대 해상도

```

옵시디언에서 사용하고 싶다면 다음과 같은 형식으로 입력하면 된다.

```
![_이름_](https://i.ytimg.com/vi/_ID_/maxresdefault.jpg)

```

## Reference

- \[How to View Youtube Thumbnail Image in High Resolution? - Orbiting Web\]( [https://orbitingweb.com/blog/view-youtube-thumbnail-image/](https://orbitingweb.com/blog/view-youtube-thumbnail-image/)
