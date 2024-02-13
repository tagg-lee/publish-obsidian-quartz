---
publishedAt: 2023-08-13T12:32:35.000Z
FeatureImage: 
---
## 문제

이 글에서는 데본씽크 3를 편의상 DT3 라고 하겠다.

필자는 옵시디언을 사용한다.

DT3의 문서를 옵시디언에 참조하고 싶을 때가 있다.

그럴 때면 DT3에서 `Copy item link` 로 그 문서의 링크를 복사한다.

그러면 요런게 복사된다.

`x-devonthink-item://abcd123`

옵시디언에서 이 링크를 써먹으려면 마크다운 형식으로 만들어줘야 한다.

바로 다음과 같이 `[Title](x-devonthink-item://abcd123)`

그러면 그 링크를 클릭했을 때 DT3의 문서로 이동된다.

그런데 문제가 있다.

마크다운 형식으로 만드는 과정이 너무 귀찮다.

(필자는 프로 귀차니스트이다.)

Title 따로 링크 따로 복사해서 마크다운 형식으로 만들어줘야한다.

필자는 이 과정을 클릭 두 번만에 하기를 바랬다.

그래서 구글링을 했고, 역시 나와 같은 불만을 가진 사람이 있었다.

이 글에서는 아래 커뮤니티의 대화에 나온 해결책을 소개하려한다.

[Markdown version of the Item link - DEVONthink](https://discourse.devontechnologies.com/t/markdown-version-of-the-item-link/55041/19)

> Thank you so Much!

![](https://images.unsplash.com/photo-1608389168343-ba8aa0cb3a63?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wxMTc3M3wwfDF8c2VhcmNofDF8fHRoYW5rfGVufDB8fHx8MTY5MTkzMDIwN3ww&ixlib=rb-4.0.3&q=80&w=2000)Photo by [Alexas\_Fotos](https://unsplash.com/@alexas_fotos?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit) / [Unsplash](https://unsplash.com/?utm_source=ghost&utm_medium=referral&utm_campaign=api-credit)

## 설정법

1. `Script Editor.app` 을 열기
2. `New Document` 로 새 문서 만들기
3. 아래의 스크립트를 입력하기

```
tell application id "DNtp"
	set theMarkdownLinks to {}
	repeat with thisRecord in (selected records)
		copy ("[" & (name of thisRecord) & "](" & (reference URL of thisRecord) & ")  " & return) to end of theMarkdownLinks
	end repeat
	if theMarkdownLinks ≠ {} then
		display notification ((count items of theMarkdownLinks) & " Markdown links copied" as string) with title "Markdown-Link(s) kopiert"
		set the clipboard to (theMarkdownLinks as string)
	end if
end tell

```

저장하기. (필자는 "DT3\_Copy as Markdown"이라 저장했다.)

스크립트를 DT3 스크립트 폴더에 넣기

a. 파인더를 열고 `cmd + shift + g` 를 누른다.

b. 다음 주소를 입력한다.

`/Users/tagg/Library/Application Scripts/com.devon-technologies.think3/Menu`

b. 이 위치에 스크립트를 저장한다.

## 사용법

### 1\. DT3의 메뉴에서 스크립트 아이콘 클릭

![](https://i.imgur.com/LeWnOMd.jpg)

스크립트 메뉴에서 선택해서 실행하는 방법이 있다.

하지만 프로 귀차니스트인 나에게는 너무 번거로운 일이다.

감사하게도, 단축키 설정이 가능하다.

### 2  단축키로 스크립트 실행하기

[CustomShortcuts](https://www.houdah.com/customShortcuts/) 라는 앱을 설치하자.

그러면 스크립트를 단축키로 설정할 수 있다.

연관글:

[맥북 커스텀 단축키 앱 2 가지\
\
서론 필자는 프로 귀차니스트다. 그만큼 생산성에 환장한다는 의미다. 이런 필자에게 단축키는 목숨과 같다. 필자가 사용 중인 단축키 설정에 도움되는 앱을 소개한다. 1\. CustomShortcuts Houdah Software의 Pierre Bernard가 만들고 무료로 배포했다.Thank you so much! 설치 및 사용 1. 아래 링크로 들어가서 설치한다. CustomShortcuts 2. 권한 설정을 한다. Settings/Privacy & Security\
\
![](__GHOST_URL__/content/images/size/w256h256/2023/08/------------------------_60-60-1.png)이태극의 지식창고이태극\
\
![](https://images.unsplash.com/photo-1526920929362-5b26677c148c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wxMTc3M3wwfDF8c2VhcmNofDN8fHNob3J0Y3V0fGVufDB8fHx8MTY5MTkyOTMwMHww&ixlib=rb-4.0.3&q=80&w=2000)](__GHOST_URL__/post-2/)![](https://i.imgur.com/K9Jmcwb.jpg)

## 감사

스크립트를 작성하고, 단축키 솔루션을 만들어주신 분들에게 감사를 표한다.

그들 덕에 편리하게 링크를 복사하고 붙여넣을 수 있다.
