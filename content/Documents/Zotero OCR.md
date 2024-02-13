---
aliases: 
created: 2023-11-04
tags: 
type: "[[How-to]]"
---

# 조테로 OCR 방법

## On Mac OS
We need:
- [Zotero OCR](https://github.com/UB-Mannheim/zotero-ocr) 
- [Homebrew](https://brew.sh/) 
- Tesseract 
- Poppler

## 설정 방법
#### 1. Zotero OCR 설치 하기
1. 마지막 버전의 XPI 파일 설치하기. 
   [Releases · UB-Mannheim/zotero-ocr](https://github.com/UB-Mannheim/zotero-ocr/releases)
2. 조테로 상단 메뉴에서 `Tools/Add-ons` 열기
3. `.XPI` 파일을 드래그해서 올린다. (`Install(3)`은 시간이 좀 지나면 누를 수 있다.)
4. `Restart Now`를 누른다.

#### 2. Tesseract와 Poppler 설치
Homebrew로 설치하는 방법.
`Terminal`에 아래 명령어를 입력한다. 
1. `brew install tesseract`
2. `brew install poppler`

> Tesseract 설치를 위해서는 `Xcode.app`가 설치돼있어야 한다. 

#### 3. Tesseract와 Poppler의 위치 찾기
`Terminal`에서 다음을 따라한다.
1. `brew list tesseract`
2. 다음과 닮은 주소를 찾아서 복사한다.
   `/opt/homebrew/Cellar/tesseract/5.3.3/bin/tesseract` 
3. `brew list poppler`
4. 다음과 같은 주소를 찾아서 복사한다.
   `/opt/homebrew/Cellar/poppler/23.10.0/bin/pdftoppm`


#### 4. Zotero OCR 설정하기
1. Zotero의 상단바에서 `Tools/Zotero OCR Preferences`를 연다.
2. `OCR parameters`에 아까 복사했던 주소를 사진과 같이 붙여넣기 한다. 
3. `Output options`는 `Save output as PDF with text layer`만 선택한다. 나머지 체크박스는 해지한다. 

## 사용 방법
1. OCR이 필요한 PDF를 찾아서 마우스 우클릭한다. 
2. `OCR selected PDF(s)`를 클릭한다. (PDF 뷰어가 켜져있으면 안된다.)


## Reference
- [04 OCR in Zotero - Doing History with Zotero and Obsidian - Obsidian Publish](https://publish.obsidian.md/history-notes/04+OCR+in+Zotero)