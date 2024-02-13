---
permalink: 
tags:
  - 🏷️Document
Keywords: 
aliases: 
description: 
updated: 
created: 2024-02-11
publish: true
---
free-tags:: 

## ...

## Cloudflare(클라우드플레어)란?


## 가이드

#### 서브 도메인으로 포워딩 하기
Reference: [How do I create a subdomain and redirect it>? - Website, Application, Performance / DNS & Network - Cloudflare Community](https://community.cloudflare.com/t/how-do-i-create-a-subdomain-and-redirect-it/74956)

Record 설정
1. "DNS > Record"로 이동
2. `Add Record` 클릭 
3. 아래와 같이 입력 후 `Save`
>    Type: `A`  
>    Name: {서브도메인}
>    IPv4: 8.8.8.8

포워딩 설정
1. "Rules > Page Rules"로 이동
2. `Create Page Rule` 클릭
3. 아래와 같이 입력 후  `Save and Deploy Page Rule` 클릭
   >URL: (예시)'sub.main.com'
   >Pick a Setting: `Forwarding URL`
   >Select status code: `301- Permanent Redirect`
   >Enter destination URL: {포워딩할 URL}`