---
aliases: 
created: 2023-10-25
tags:
  - Obsidian-app
---
Up:: [[Obsidian Plugin_Tasks Documentation]]

# 반복되는 Task 만들기

#### 1  명령어 팔레트 열기
단축키: `CMD + P`

\
\
\
	

#### 2  명령어 실행 `Tasks: Create or edit task`

![|550](https://i.imgur.com/BCDyITV.png)


\
\
\
	

#### 3 Task 설정 방법
1. `Recurs`에 반복 주기를 입력한다.
2. Due 또는 Scheduled에 시작일을 입력한다.

**Image 1**
![|325](https://i.imgur.com/rUzGCxv.png)

\
\
\
	

자연어(natural language) 기능이 있다.
그래서 `Friday`라고 입력하면 가장 최신 금요일의 날짜를 입력한다.

**Image 2**
![|375](https://i.imgur.com/z7VQCZD.png)

\
\
\
	
#### 4 결과
그러면 다음과 같은 결과물이 생긴다. 
완료 처리를 하면 위 또는 아래에 새로운 날짜로 생성된다.
아래 설정을 통해 위 또는 아래로 설정할 수 있다.

![|450](https://i.imgur.com/KmRIDM5.png)



지금은 `Recurs`를 `Every day`라고 했기에 Task를 완료했을 때 일자에 +1이 된다.
만약 `Every two days`라고 했으면 +2 가 되어 생성될 것이다.

```
- [ ] #TODO 아침에 산책하기 🔁 every day 📅 2023-10-28
- [x] #TODO 아침에 산책하기 🔁 every day 📅 2023-10-27 ✅ 2023-10-25
```


