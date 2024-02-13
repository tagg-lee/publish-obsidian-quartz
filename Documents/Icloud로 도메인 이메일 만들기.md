---
publish: true
permalink: create-domain-email-with-iCloud
created: 2023-11-20
updated: 
description: 
aliases: 
status: 
tags: 
---
Up:: 

## 준비물
- Icloud (이메일 호스팅)
- Cloudflare (도메인 관리)
- Gmail (이메일 클라이언트)

# 방법
### 1. Icloud로 도메인 이메일 호스팅하기

1. 아이클라우드 웹 들어가기
2. 도메인 등록하기
3. 도메인 레지스터 설정하기
	1. Cloudflare에 레코드 입력하기
	2. (중요!) `DNS Only`로 설정하기 
4. 도메인 이메일 주소 생성하기

### 2. Spark와 연동하기
1. `APP-SPECIFIC PASSWORDS` 생성하기
2. Spark에 Email과 `APP-SPECIFIC PASSWORDS` 입력하기

## 설정 팁
- Junk mail을 Inbox로 보내기
- 


# Reference
- [Solved: How-To Use Gmail SMTP to Send FROM an Email Address which uses Cloudflare Email Routing - Website, Application, Performance / Getting Started - Cloudflare Community](https://community.cloudflare.com/t/solved-how-to-use-gmail-smtp-to-send-from-an-email-address-which-uses-cloudflare-email-routing/382769)
	- 1. Cloudflare에서 Forwarding 하는 방법
	- 2. Gmail에서 도메인 이메일로 회신하는 방법
- [iCloud Mail Forwarding - some emails aren… - Apple Community](https://discussions.apple.com/thread/254699789)
	- iCloud Mail에서 Gmail로 Forwarding이 안되는 이유.
- [How to Add iCloud Email to iPhone or iPad](https://sparkmailapp.com/add-icloud-ios)
	- iCloud mail과 Spark 연동하는 방법