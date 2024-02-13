---
aliases: 
created: 2023-10-17
type: 
tags: 
---


# 마크다운 | URL에 닫힌 괄호 ')'가 들어갔을 때

마크다운의 외부 링크 연결 문법은 `[name](url)`이다. 
그래서 만약 url에 닫힌 괄호가 들어가면 url이 잘리게 된다. 

>[!note] 예시
> 입력: `[이태극의 프로필](https://profile).tagglee.me)`
> 결과: [이태극의 프로필](https://profile).tagglee.me)

닫힌 괄호를 Encode 해서 입력하면 해결된다. 
`) = %29`

## Reference
- https://stackoverflow.com/questions/13824669/how-do-you-write-a-link-containing-a-closing-bracket-in-markdown-syntax