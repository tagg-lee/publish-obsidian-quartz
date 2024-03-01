---
permalink: quartz-jzhao-xyz
tags:
  - 🏷️Document
Keywords:
  - "[[소프트웨어 개발(Software Development)]]"
aliases: 
description: 
updated: 
created: 2024-02-10
publish: true
---
free-tags:: #open-source #blog 

## Summary
- [Quartz 4](https://quartz.jzhao.xyz/)는 오픈소스 ==정적 웹사이트 생성기(static site generator)==이다.
- Features
	- Markdown
	- Graph view
	- Full-text search engine
- Similar Conversions
	- Hugo
	- Jekyll

##### Recommended contents 
- [Quartz v4: a free Obsidian Publish alternative : ObsidianMD](https://www.reddit.com/r/ObsidianMD/comments/15wryj2/quartz_v4_a_free_obsidian_publish_alternative/)
- [How to publish your notes for free with Quartz - YouTube](https://www.youtube.com/watch?v=6s6DT1yN4dw)
	- What is Quartz?
	- Who use this for?
	- How set-up?
		- [How to publish Obsidian notes with Quartz on GitHub Pages - Fork My Brain](https://notes.nicolevanderhoeven.com/How+to+publish+Obsidian+notes+with+Quartz+on+GitHub+Pages)


## Hosting Obsidian notes on Github Pages
References
- [How to publish your notes for free with Quartz - YouTube](https://www.youtube.com/watch?v=6s6DT1yN4dw)
- [How to publish Obsidian notes with Quartz on GitHub Pages - Fork My Brain](https://notes.nicolevanderhoeven.com/How+to+publish+Obsidian+notes+with+Quartz+on+GitHub+Pages)
- [Welcome to Quartz 4](https://quartz.jzhao.xyz/)

### 방법 1
**준비물**: 
- Obsidian
- Github
- Node.js
	- 권장
		- Node: 21.6.0
		- **(2024.01 기준 21.6.0 이상 버전 사용 시 에러 발생)**
	- 최소: 
		- Node:  v18.14
		- npm: v9.3.1


#### Steps
###### 1_ Quartz 4를 설치할 폴더를 생성한다. 


###### 2_ 터미널을 키고 해당 폴더로 이동한다. 


###### 3_ Download a copy of the Quartz repository
```
git clone https://github.com/jackyzha0/quartz.git
```


###### 4_ Rename `quartz` to `Publish`
```
mv quartz Publish
```


###### Change the directory to the new folder
```
cd Publish
```


###### 5_ Use NPM to install those dependencies
```
npm i
```


###### Create new Quartz project
```
npx quartz create
```


###### 두 가지 옵션을 설정한다. 
1. Method of initializing
```
- Empty Quartz  (이거 선택)
- Copy an existing folder
- Symlink an existing folder
```

2. Choose how Quartz should resolve links in your content. 
```
- Treat links as absolute path
- Treat links as shortest path (이거 선택)
- Treat links as relative paths
```
You can change this later in `quartz.config.ts`.


###### Check origin remote
```
git remote -v
```


###### Remove default origin remote
```
git remote rm origin
```


###### Change origin remote
```
git remote add origin https://github.com/<yourusername>/<repositoryname>.git
```


###### Pushing the changes to remote repository(github)
```
npx quartz sync --no-pull
```


###### Build your site locally
```
npx quartz build --serve
```


###### Enter `ctrl + C`  to stop server.


###### Sync to Github
```
npx quartz sync
```

###### Make a file `.github/workflows/deploy.yml` 
and paste codes at https://quartz.jzhao.xyz/hosting#github-pages


###### Setting Github Actions
```
Github > Setings > Pages > Source > (Select) Github Actions
```

>[!warning] 반드시 순서를 지키세요.
>이 단계의 설정을 마치지 않고 다음 단계로 넘어가면 에러가 발생합니다. 
>반드시 `Setting Github Actions`**을 먼저 완료**한 뒤 16번 스텝으로 넘어가세요. 



###### Create GitHub Action
```
npx quartz sync
```

#### 방법 2 by 안피곤
[옵시디언 무료 퍼블리시 방법(👍추천): Cloudflare, Quartz, Flowershow Plugin](https://anpigon.tistory.com/m/449)