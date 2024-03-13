---
title: Google Sheets(구글 시트)
permalink: 
tags:
  - 🏷️Document
  - 📦App
Keywords: 
aliases: 
description: 
updated: 
created: 2024-02-13
publish: true
---
free-tags:: #Office
</br>
</br>

## ...

## 개요
- Google에서 만든 워크스페이스 중 하나다. 

## Tips
#### 캘린더 팝업 뜨게 만들기

1. `Data validation rules` 켜기
   위치: `Data > Data validation`
2. `Add rule`을 클릭하기 
3. `Apply to range`에서 적용 범위 입력
4. 드롭다운 `Criteria`에서 `Is valid date` 선택
5. `If the data is invalid:`에서 `Reject the input`


Reference: [Google Sheets - Add a Pop-Up Calendar Date Picker - YouTube](https://www.youtube.com/watch?v=7ywMarY4oNQ)

#### 다른 시트 불러오기
##### Functions
- `importrange()`
- `query()`


#### 필터된 값만 계산하기
Reference:
- [How to Sum Filtered Rows in Google Sheets (With Examples) - Statology](https://www.statology.org/google-sheets-sum-filtered-rows/)
- [SUBTOTAL function - Google Docs Editors Help](https://support.google.com/docs/answer/3093649?hl=en)


#### 문자열 "60/40"의 숫자 각각 골라내기
```formula
=VALUE(LEFT(G3, FIND("/", G3) - 1))
```
- `VALUE()`
	- 문자열을 숫자로 변환합니다. 문자열과 달리 숫자는 산수가 가능합니다. 
- `LEFT(문자열, 문자_위치_값)`
	- `LEFT()` 함수는 입력받은 `문자열`의 시작점부터 입력받은 `문자_위치_값`까지의 문자만 반환합니다. 
	- 예시: `LEFT("1234567", 3)`는 "123"을 반환합니다. 
- `FIND("/", G3)`
	- 문자열 'G3'에서 "/"의 위치 값을 반환합니다. 
	- 마지막에 `-1` 을 해서 "/"의 왼쪽에 위치한 문자 위치 값을 구했습니다. 


```formula
=VALUE(MID(G3, FIND("/", G3) + 1, LEN(G3) - FIND("/", G3)))
```
- `MID(문자열, 문자_위치_값_시작, 문자_위치_값_끝)`
	- `MID()` 함수는 입력받은 `문자열`의 입력받은 시작점과 끝점 사이 문자열을 반환합니다. 
	- 예시: 예시: `LEFT("1234567", 2, 5)`는 "2345"을 반환합니다. 


## Functions

#### ARRAYFORMULA(array_formula)
>###### EXAMPLE
>ARRAYFORMULA(A1:C1+A2:C2)
>
>###### ABOUT
> Enables the display of values returned from an array formula into multiple rows and/or columns and the use of non-array functions with arrays.
>
> ---
> `array_formula`
> A range, mathematical expression using one cell range or multiple ranges of the same size, or a function that returns a result greater than one cell.
> 
> [Learn more](https://support.google.com/docs/answer/3093275?hl=en&sjid=9124382006651170583-AP#null)

##### Resources
- [Google Sheets - Use ARRAYFORMULA Instead of Repeating Functions - YouTube](https://www.youtube.com/watch?v=92C3V0GjhgA)