---
publishedAt: 2023-09-18T08:12:27.000Z
FeatureImage: 
---
## What is Smart Connections

옵시디언의 커뮤니티 플러그인으로, gpt API를 활용한 기능을 제공해요.

이 플러그인을 활용하면 노트하는 과정이 더 쉽고 재밌어질 수 있어요.

서로 관련성 있는 노트를 찾고 연결하는 과정은 에너지가 꽤 많이 들어요.

하지만 Smart Connections를 활용하면 부담을 줄일 수 있어요.

AI가 알아서 찾아주거든요!

저는 종종 "오~ 이렇게 연결될 수 도 있내!"라는 경험을 해요.

자, 그럼 Smart Connections에 어떤 기능이 있는지 아래에서 자세히 알아보아요.

플러그인 설치하기

## Features

1. Smart Chat
2. Smart View
3. External Connections

### 1\. Smart Chat

![](https://i.imgur.com/zAIN24E.gif)

Smart Chat은 내 노트로 AI와 대화할 수 있는 기능이에요.

Smart chat을 활용해서 여러 노트의 내용을 정리 및 요약을 한다거나,

노트간의 연결성을 만들어 새로운 아이디어를 만들 수 있어요.

GPT-4 API를 연동하면 더 좋은 퀄리티의 답변을 얻을 수 있어요.

다만, 더 비싸겠죠?

#### Smart Chat을 여는 방법

1. `Command Palette` 를 열어 "Smart Connections: Open Smart Chat"을 실행하세요. `Command Palette` 을 여는 단축키는 `cmd/ctrl + P` 에요.
2. 만약 `Smart View` 가 이미 열려있다면, 우측 상단에 채팅 아이콘을 클릭하세요.

#### 내 노트를 참고시키는 여러가지 방법

> \# 하나의 노트로 대화하기
>
> \[\[비트겐슈타인의 논리철학논고에 대하여\]\] 노트를 요약해줘.

> #여러 노트로 대화하기
>
> \[\[카오스 이론과\]\] \[\[조직과 결정 \- 니클라스 루만\]\] 노트의 관계를 설명해줘.

> #특정 폴더 안의 노트로 대화하기
>
> /Reference 폴더 안의 노트들을 참고해서 내가 가장 관심을 갖는 분야가 뭔지 알려줘.

> #노트 안의 특정 내용으로 대화하기
>
> \[\[비폭력대화\]\]의 "나의 생각"이란 Heading의 내용을 요약해 줘.

#### 추가될 기능

만약 AI 답변이 내 노트를 참고해서 대답할 경우에 그 노트의 링크를 제공할 거라고 해요.

마치 Bing chat이 답변에 참고한 웹사이트 링크를 알려주듯이요.

### 2\. Smart View

![](https://i.imgur.com/z2uCeBf.png)

원래 우리는 서로 관련된 노트를 직접 찾아서 연결해야 했어요.

하지만 Smart View는 AI가 서로 관련된 노트를 알아서 찾아서 보여줘요.

결과물이 꽤 괜찮아요. 실제로 내가 연결했을 법한 노트들을 추천해주거든요.

그리고 창의적인 연결이 생겨서 아이디어를 얻을 수 도 있어요.

#### Smart View: Find

Smart view의 우측 상단에 검색 아이콘을 클릭하면 검색할 수 있어요.

키워드나 어구 또는 문장을 입력하면 그와 연결된 노트를 찾아서 리스트로 보여줘요.

이 때 노트 안에 하이라이트된 내용을 사용한다고 해요.

제 볼트에서 "집중력을 높이기 위해서 무엇을 해야하나요?"라고 입력했을 때 나온 결과에요.

![](https://i.imgur.com/qJ7hUhG.png)

#### Smart View: Dynaic Code Block

코드 블록을 사용해서 `Smart View: Find` 를 노트 안에 만들 수 있어요.

방법은 다음과 같아요.

> \`\`\`smart-connections
>
> {{검색어}}
>
> \`\`\`

{{검색어}}을 `Smart View: Find` 에서 입력할 때와 같이 사용하면 돼요.

### 3\. External Connections

내 옵시디언 볼트 밖의 외부의 정보를 사용할 수 있어요.

예를들어 내 이메일과 연동하거나 블로그의 글을 참고할 수 있는 거죠.

이 기능은 앞으로 추가될 예정이라고 해요.

## Reference

- [brianpetro/obsidian-smart-connections: Chat with your notes in Obsidian! Plus, see what's most relevant in real-time! Interact and stay organized. Powered by OpenAI ChatGPT, GPT-4 & Embeddings. (github.com)](https://github.com/brianpetro/obsidian-smart-connections)
- [Introducing Smart Chat: Transform Your Obsidian Notes into Interactive AI-Powered Conversations with GPT-4 & Embeddings - WFH Brian](https://wfhbrian.com/introducing-smart-chat-transform-your-obsidian-notes-into-interactive-ai-powered-conversations/)

Smart connections를 개발해주셔서 감사합니다 🥰
