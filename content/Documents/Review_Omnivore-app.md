---
publishedAt: 2023-09-05T03:26:23.000Z
FeatureImage: 
tags:
  - Productivity
  - PKM
---
type:: [[Review]]
# 무료 Read it later 최강자 Omnivore 옴니보어
## 옴니보어 설명회 영상

유튜브 페이지에서 설명란 참고하세요.

## Omnivore란?

Read it later 앱 중에 하나이. Read it later은 말 그대로 글을 나중에 읽는 것을 돕는 서비스이다. 이 서비스들의 공통적인 기능은 다음과 같다.

- 다양한 형식의 글들을 한 곳에 저장할 수 있다. (Web article, Newsletter, RSS, PDF 등)
- Label 또는 Folder으로 글들을 분류할 수 있다.
- 내 저장소에 보관되기 때문에 인터넷에 글이 삭제되더라로 문제 없다.
- 글을 읽으며 하이라이트나 노트를 할 수 있다.
- 다양한 플랫폼에서 지원한다. (Web, WIndow, Mac, Android, IOS)

옴니보어의 특별한 특징은 무료 오픈소스 서비스라는 것이다. 만약 개발을 조금 할 줄 안다면 더 다양한 활용성을 갖게 된다. 마치 옵시디언처럼 커뮤니티가 활발해져서 다양한 기능이 생기길 바래본다.

옵시디언에 옴니보어 플러그인이 있다. 그래서 옴니보어에 저장된 글, 하이라이트, 노트들을 옵시디언으로 불러올 수 있다.

![](https://i.imgur.com/bjC8pCk.png)

## Readwise Reader를 떠난 이유

나는 원래 월 9$ 내고 Readwise Reader를 구독 중이었다. Omnivore를 알고 있었지만 Reader에 비해 사용성이 많이 부족해서 쓰지 않고 있었다. 그럼에도 옴니보어로 옮기게된 이유는 다음과 같다.

### 구독료가 아깝다

요즘 바쁜 관계로 Reader에 쌓인 글들을 잘 읽지 않다보니 구독료가 너무 아까웠다.

그러다보니 더 편리한 기능의 매력이 떨어졌다. 조금 불편하더라도 내게 꼭 필요한 기능이 있으며 무료인 옴니보어로 옮기기로 결정했다.

### Full Contents

Reader에서 옵시디언으로 글을 불러올 때 하이라이트만 가져온다. 하지만 옴니보어는 하이라이트 뿐만 아니라 컨텐츠 내용 전체를 가져올 수 있다. 이는 내게 굉장히 매력적이었다. 왜냐면 나는 Reader에 저장한 글들을 모두 내 컴퓨터에 저장하고 싶은데 그러기 어려웠기 때문이다. 앞으로 Reader에서 이걸 편리하게 할 수 있도록 지원해줄 지는 모르겠지만, 이미 내 마음은 떠나버렸다.

## 옴니보어의 단점

아직 개발 단계라서 부족한 점들이 있다. 현재 내가 발견한 불편들을 몇 가지 뽑아본다면 다음과 같다.

- '제로 인박스'를 하기에는 불편한 UX (나의 가장 큰 불만이다)
- RSS Feed 등록 버튼이 없음(업데이트 예정)
- Query 커스터마이징 미지원 (업데이트 예정)
- 모바일과 PC 앱의 완성도 떨어짐

## 옵시디언 옴니보어 플러그인 세팅

위 유튜브 영상 14:40의 설명을 보고 따라하면 된다.

### Article Template

```
[[Omnivore MOC]] | [Read on Omnivore]({{{omnivoreUrl}}}) | [Read Original]({{{originalUrl}}})
{{fileAttachment}}

{{# note }}
# Note
{{note}}
{{/ note }}

{{#highlights.length}}
# Highlights

{{#highlights}}
> {{{text}}} [⤴️]({{{highlightUrl}}}) {{#labels}} #{{name}} {{/labels}} ^{{{highlightID}}}
{{#note}}

    📝 {{{note}}} {{/note}}
{{/highlights}}
{{/highlights.length}}

# Full Contetns
{{{ content }}}
```

### Front matter template

Setting창 맨 아래에 `Advanced setting` 의 안에 있다.

```front
fileClass: Omnivore
id: {{{id}}}
type: {{type}}
{{#author}}
author: {{{author}}}
{{/author}}
{{#labels.length}}
tags:
{{#labels}} {{{name}}}
{{/labels}}
{{/labels.length}}
{{#datePublished}}
date_published: {{{datePublished}}}
{{/datePublished}}
date_archived: {{dateArchived}}
state: {{state}}

```
