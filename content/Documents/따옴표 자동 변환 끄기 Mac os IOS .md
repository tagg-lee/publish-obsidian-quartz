---
publishedAt: 2023-09-04T07:43:47.000Z
FeatureImage: 
---
## 개요

CSS를 작성하는데 자꾸 오류가 났다. 왜 그런건지 한참을 찾고 보니 따옴표에 문제가 있었다.

나는 `"` 이걸 입력했는데 `“ ` 이렇게 바뀌어 있었다. 즉, 열림 따옴표로 변환된 것이다.

컴퓨터 프로그래밍할 때 `' '` 나 `" "` 를 자주 사용하는데 이렇게 자동 변환되버리면 곤란하다. 모양도 비슷해서 찾기 힘들다. 변환 안되는 방법 없을까 찾아보았다. 역시나 방법은 있었다.

방법은 **Smart puctuation(스마트 구두점)** 기능을 끄면 된다.

(이 글은 Mac OS를 위한 글이다. 만약 Windows에서 문제를 겪고 있다면 이 글에서 키워드를 얻길 바란다.)

# Mac os 방법

### 1\. 설정창으로 이동한다.

설정창 위치는 다음과 같다. `Preference > Keyboard > Text Input 아래의 Edit`

스포트라이트에 `Use smart quotes and dashes` 을 검색해서 들어갈 수 도 있다.

![](https://i.imgur.com/t6X97Jq.png)

### 2\. "For double quotes"와 'For single quotes'의 설정을 바꾼다.

기본 설정을 자세히 보면 열림과 닫힘으로 되어있다. 대신에 가장 아래에 있는 옵션을 선택하자.

![](https://i.imgur.com/2ADQx8F.png)

# IOS 방법

![](__GHOST_URL__/content/images/2023/09/image.png)[Tips: Turn off iOS 11 Smart Punctuation to avoid data entry problems \| AppleInsider](https://appleinsider.com/articles/17/09/26/tips-turn-off-ios-11-smart-punctuation-to-avoid-data-entry-problems)

**설정 -> 키보드 -\> 스마트 구두점**

## Reference

- [macos - How to disable smart quotes - Ask Different (stackexchange.com)](https://apple.stackexchange.com/questions/136402/how-to-disable-smart-quotes)

  Thanks for the help!
