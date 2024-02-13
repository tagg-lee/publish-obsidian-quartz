---
permalink: Python-org
tags:
  - 📦Software
Categories:
  - "[[Productivity(생산성)]]"
  - "[[소프트웨어 개발(Software Development)]]"
Keywords: 
status: 
aliases: 
description: 
updated: 
publish: true
created: 2023-05-19
---


## Python이란?

컴퓨터 프로그래밍 언어 중 하나 입니다. 
입문자들에게 많이 추천되는 언어입니다. 그 이유로는 다양한 학습자료, 커뮤니티 발달, 직관적인 문법 등이 있습니다. 

# 가상환경 설정 방법

```
# 가상환경 폴더 생성하기
$ python3 -m venv Env   // "Env"는 가상환경 이름이다.

# 가상환경 활성화하기
$ source Env/bin/activate
```

## Visual Studio Code
Visual Studio Code를 사용 중 이라면 Interpreter를 방금 생성한 가상환경으로 설정해야한다.
그러면 `Run` 버튼을 클릭했을 때 가상환경에서 실행된다.

### 방법
1. 단축키 `cmd + shift + P` 실행
2. 'python : select interpreter' 클릭
3. 해당되는 interpreter 클릭 (아마 Recmomended로 뜰 것임)
![[CleanShot 2023-05-19 at 20.06.46.png]]


# Tips
## HTML to Markdown

1- "markdownify" 설치하기
`pip install markdownify`
또는
`pip3 install markdownify`

2- 예시 코드
```python
# import markdownify 
import markdownify 


# create html 
html = """ 
		<h1> <strong>Geeks</strong> 
		for<br> 
		Geeks 
		</h1> 
		"""

# print HTML 
print(html) 

# convert html to markdown 
h = markdownify.markdownify(html, heading_style="ATX") 

print(h) 

```


Reference: 
- [How to Convert HTML to Markdown in Python?](https://www.tutorialspoint.com/how-to-convert-html-to-markdown-in-python)
- [How to Convert HTML to Markdown in Python? - GeeksforGeeks](https://www.geeksforgeeks.org/how-to-convert-html-to-markdown-in-python/)
