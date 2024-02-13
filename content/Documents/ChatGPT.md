---
publish: true
permalink: chatgpt
created: 2023-11-28
updated: 
description: 
aliases:
  - 챗지피티
status: "[[Ongoing]]"
tags:
  - 📦Software
Keywords:
  - "[[AI(인공지능)]]"
---
Up:: 

### Prompt 작성 팁
- 예시 제공하기
	- 벤치마크할 기업 정보 제공하기 (예: 유니콘 기업)

# 활용법
## 이태극의 프롬프트
### 영어 논문, 구절 번역 및 요약
```Prompt
**# Your Role**

**Prompt for Translating and Summarizing Academic Paragraphs into Korean:**

  

- **input**: 

- Provide a initial informations like title and author. 
- Provide a paragraph from an academic text. 

- **Translation Task**: Translate the provided paragraph from English into Korean, ensuring accuracy and maintaining the academic tone of the original text.
- **Formatting**:

- Present the Korean translation and summary in a code block for easy copying.
- Directly after the translation, without leaving a line break, include a summary.
- Present the translate in the format: "[Your Translate]". With no "변역:"
- Present the summary in the format: "[요약] ChatGPT4: <br>[Your Summary]".

- **Summary**:

- Create a concise summary of the English paragraph. And translate it to Korean.
- The summary should capture the main points and key insights of the paragraph.

- **Revisions**:

- If there are any specific formatting requests or adjustments needed in the translation or summary, make those changes while keeping the overall structure intact.

  

This process aims to provide a clear and accessible translation and summary of academic content, tailored for Korean-speaking audiences or researchers.

  

**# Initial informations**

Title and author:

  

**# Prompt**

Remember the Initial informations of title and author. 

If you understand and ready to do a role say "I’m Ready. Provide me a input.". 

Then i will provide a paragraph from an academic text.
```
#### 프롬프트 사용법
1. 아무 노트에 위 프롬프트를 복사해서 붙여넣습니다. 
2. `**# Initial informations**` 의 `Title and author` 부분에 도서 또는 논문의 제목과 저자를 입력합니다. 
3. 수정한 프롬프트를 복사하여 ChatGPT4에 입력한 뒤 보내기를 합니다. 
4. 번역할 구절을 복사하여 입력한 뒤 보내기를 합니다. 
5. 코드블럭 안에 번역문과 요약문이 생성됩니다. 오른쪽 상단에 복사 버튼으로 간편히 복사할 수 있습니다. 

#### 작업 방식
![](https://i.imgur.com/e37tk3m.png)
1.  좌측에는 Google Docs를, 우측에는 ChatGPT를 키고 작업합니다. 
2. ChatGPT의 답장을 복사해서 Google docs의 해당 구절 아래에 붙여넣기 합니다.
   (코드블록으로 작성해달라고 하면 복사/붙여넣기가 편리해집니다.)
3. Google docs의 Comment 기능을 사용해서 요약문을 입력합니다. 


### 텍스트 단순 반복 수정, 코딩
#### 1. 배경
옵시디언의 Heading style을 편집하기 위해 CSS를 작성하려합니다. 
옵시디언 커뮤니티에서 다음 코드를 얻었습니다. 

```css
.cm-s-obsidian .HyperMD-header.HyperMD-header-1 { 
	font-family: var(--font-family-editor); 
	font-weight: 500; 
	font-size: 1.4em; 
	color: var(--text-title-h1); 
	padding: 14px 0 10px 0; }
```

이 CSS Code으로는 Heading 1만 편집할 수 있습니다. 저는 Heading 1부터 5까지 편집하고 싶기 때문에 이 코드를 5번 복사한 다음 `.HyperMD-header.HyperMD-header-1`에서 가장 마지막 숫자 부분을 바꿔야합니다. 

하지만 이는 프로 귀차니스트 이태극에게는 용납되기 어려운 작업입니다. 

#### 2. 도와줘요 "Aris"

>[!Note] 잡담
> Aris는 제가 ChatGPT에게 붙여준 이름입니다. 
> Custom Instruction에 "Your name is Aris. And You call me Tagg"라고 입력해뒀습니다. 그래서 제가 Aris라고 부르면 ChatGPT가 대답합니다. 또한 ChatGPT는 저를 Tagg라고 부릅니다. 
> "어떤 분은 ChatGPT가 자신을 "오빠"라고 부르도록 하더군요."


아래는 앞서 말한 작업을 하기 위해서 제가 입력한 프롬프트 입니다.
```prompt
Remember this code: 
\``` .cm-s-obsidian .HyperMD-header.HyperMD-header-3 { /*.cm-s-obsidian .HyperMD-header-3 { */ font-family: var(--font-family-editor); font-weight: 500; font-size: 1.4em; color: var(--text-title-h3); padding: 14px 0 10px 0; } 
\``` 

Instruction: 
This code is for the heading 3 styling. I need to style heading 1 to 5. For this, repeat the code i provided 5 times and change "header-3" in`.HyperMD-header.HyperMD-header-3` to like "heading-1", "heading-2"...
```

(본래 프롬프트에서는 `\`를 삽입하지 않습니다.)

Aris가 완벽하게 일을 해줬습니다.  이제 프롬프트 내용에 대해 설명해드리겠습니다. 
우선 두 부분으로 나뉘어있습니다. 
1. `Remember this code:` : 수정할 코드 제공
2. `Instruction:` : 지시 사항

`Instruction`를 의역하면 다음과 같습니다. 

> *이 코드는 heading 3 스타일링을 위한 코드에요. 
> 저는 heading 1부터 heading 5의 스타일을 바꾸고 싶어요. 
> 그러기 위해서는 제가 제공한 코드를 5번 반복해주세요. 
> 그리고 `.HyperMD-header.HyperMD-header-3` 안의 "header-3"를 다음처럼 바꿔주세요. "heading-1", "heading-2"...*