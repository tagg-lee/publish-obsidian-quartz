---
permalink: Review_CustomShortcuts-app
tags:
  - 🏷️Document
Keywords:
  - "[[Productivity(생산성)]]"
  - "[[Publish/content/Documents/MacOS|MacOS]]"
aliases: 
description: 
updated: 
publish: true
created: 2023-10-13
---
맥 os 단축키 환장하는 사람이라면 반드시 설치해야 할 앱


## 서론

필자는 프로 귀차니스트다.

그만큼 생산성에 환장한다는 의미다.

이런 필자에게 단축키는 목숨과 같다.

필자가 사용 중인 단축키 설정에 도움되는 앱을 소개한다.

\
\
\
	

## 1\. CustomShortcuts

### a. 장점

1. **특정 앱 기능의 단축키를 설정할 수 있다.**
2. **또한 이미 지정된 단축키를 수정할 수 도 있다.**

필자는 [옵시디언](__GHOST_URL__/tag/obsidieon/) 을 사용하며 단축키를 잘 활용한다.

그래서 **옵시디언의 단축키와 다른 앱의 단축키를 통일** 하려 한다.

예를들면, 사이드 바의 경우 \`shift + cmd + \[\` 으로 지정한다.

Houdah Software의 Pierre Bernard가 만들고 무료로 배포했다.

Thank you so much!

\
\
\
	

## 2. 설치 및 사용

1. 아래 링크로 들어가서 설치한다.

   [CustomShortcuts](https://www.houdah.com/customShortcuts/)

2\. 권한 설정을 한다.

> Settings/Privacy & Security /Full Disk Access
>
> Settings/Privacy & Security /Accessibility

3\. 단축키 설정하고 싶은 앱 클릭

4\. `Menu Item title` 에 설정할 명령어를 입력한다.

5\. 우측에 `Record Shortcut` 을 클릭하고 단축키를 입력한다.

![](https://i.imgur.com/K9Jmcwb.jpg)


\
\
\
	

## 3. 작동 원리

맥 OS 상단 바에는 File Edit View 등의 리스트가 있다. 이 안에 기능들과 기능의 단축키가 있다. **CustomShortcuts는 상단 바에 표시되는 기능들을 호출할 수 있다**.

Safari로 예를 들어보겠다.

\
\
\
	

1: `Bookmarks Sidebar` 을 끈 상태에서 `View` 를 보면 `Show Bookmarks Sidbar` 이라고 뜬다. 그리고 CustomShortcuts에 "Sidebar"라고 검색했을 때 `Show Bookmarks Sidebar` 이 검색된다.

![](https://i.imgur.com/95BHTpo.png)

\
\
\
	

2: 이번에는 `Bookmarks Sidebar` 를 켰다. 그랬더니 `View` 를 보면 `Hide Bookmarks Sidbar` 이라고 뜬다. 그리고 CustomShortcuts에 "Sidebar"라고 검색했을 때 `Hide Bookmarks Sidebar` 이 검색된다.

![](https://i.imgur.com/7AuIaN9.png)

결론: **CustomShortcuts는 상단 바에 표시되는 기능을 호출해 온다** 고 유추할 수 있었다. 그리고 단축키를 변경했을 때 상단 바에도 변경 사항이 반영되는 것을 확인했다.

단축키를 삽입하거나 편집하고 싶다면, **상단 바에서 기능의 이름을 확인** 하면 된다.

\
\
\
	

#### 참고
단축키 설정은 `System settings/Keyboard/Keyboard Shortcuts/App Shortcuts`에 저장된다.

![](https://i.imgur.com/WhWMeAT.png)


\
\
\
	


## 4. 검색 방법
내가 직접 해본 예시를 보여주려한다. 

필자는 `Craft.app`을 할 일 관리와 메모 용도로 사용한다. Block을 위 아래로 이동하는 단축키를 바꾸고자한다. 상단의 옵션 바에서 찾아보니 위치는 `Edit -> Move -> Move Up`이었다. 

![[img.Review_CustomShortcuts-app 1.jpg|500]]


\
\
\
	

이제 CustomShortcuts.app을 열어서 차근히 입력하면 된다.

1. `Edit`을 입력하면 드롭다운에서 `Edit`을 선택한다. 
2. 그러면 `Edit ->` 으로 바뀌면서 `Edit` 안에 있는 리스트를 보여준다. `Move`를 입력해서 선택한다. 
3. 앞 단계와 마찬가지다. `Move Up`을 찾아서 입력한다.  그러면 최종적으로 다음과 같이 된다. `Edit -> Move -> Move Up`
4. 우측에 버튼을 통해 단축키 설정을 한다.

`Move Down`도 위 단계와 똑같이 하면 된다.

![|500](https://i.imgur.com/YkPqise.png)
