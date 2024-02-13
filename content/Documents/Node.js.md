---
permalink: nodejs-org
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
- open-source, cross-platform [[Javascript]] runtime environement
- https://nodejs.org/en


### How to install(feat.ChatGPT)
#### Using Homebrew:
1. **Install Homebrew**: If you haven't already installed Homebrew, you can do so by executing the following command in your terminal:
    bashCopy code
    `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. **Install Node.js and npm**: Once Homebrew is installed, you can use it to install Node.js and npm:
    Copy code
    `brew install node`
#### Using Node Version Manager (nvm):

1. **Install nvm**: If you prefer managing multiple Node.js versions or want more control over the installation process, you can use nvm. First, install nvm by running:
    bashCopy code
    `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash`
2. **Close and Reopen Terminal**: After installing nvm, close and reopen your terminal to start using it.
3. **Install Node.js and npm**: Now, you can use nvm to install the latest version of Node.js and npm:
    Copy code
    `nvm install node`
    This command installs the latest LTS (Long Term Support) version of Node.js, which includes npm.

#### Verifying Installation:

After installation, you can verify that Node.js and npm are installed correctly by running the following commands:

Copy code

`node -v npm -v`

These commands should output the versions of Node.js and npm installed on your system, respectively.

By following one of these methods, you should be able to install the latest version of Node.js and npm on your macOS system.

#### 버전이 다르게 조회될 때

>[!Note] (2024-02-11)
>이 **문제의 해결은 중지 상태**입니다. 
>저는 homebrew의 Node.js를 메인으로 사용하고 싶었지만, NVM이 메인으로 설정된 상황을 어떻게 고쳐야할지 몇 시간 째 해맸습니다. 
>Homebrew를 메인으로 사용하는 것은 현재로써 중요한 일이 아니기에, 더 이상의 시간 할애를 멈춥니다. 

문제 상황
1. `brew install node`로 node.js의 최신 버전을 설치했음. 
2. 그런데 `node -v`으로 버전을 확인하면 구 버전이 조회 됨

##### 해결 방법 1
1. home brew의 node 버전 확인하기:
   `brew list --versions node`
2. 환경 변수 확인하기
	1. 실행: `echo $PATH`
	2. 결과
	   ```
	   /Users/tagg/.nvm/versions/node/v16.20.1/bin:/Users/tagg/.rbenv/shims:/opt/homebrew/bin:/opt/homebrew/sbin:/Library/Frameworks/Python.framework/Versions/3.10/bin:/opt/local/bin:/opt/local/sbin:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/Library/Apple/usr/bin
		```
		첫 번째 줄: */Users/tagg/.nvm/versions/node/v16.20.1*
3. `brew unlink node && brew link node`
4. 터미널 다시 시작하기


##### 해결 방법 2
`nvm`이 homebrew 대신 사용되는 경우가 있습니다. 
`echo $PATH`로 확인하실 수 있습니다. 

```
/Users/tagg/.nvm/versions/node/v16.20.1/bin:/Users/tagg/.rbenv/shims:/opt/homebrew/bin:/opt/homebrew/sbin:/Library/Frameworks/Python.framework/Versions/3.10/bin:/opt/local/bin:/opt/local/sbin:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/bin:/bin:/usr/sbin:/sbin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/local/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/bin:/var/run/com.apple.security.cryptexd/codex.system/bootstrap/usr/appleinternal/bin:/Library/Apple/usr/bin
```
첫 번째 줄: */Users/tagg/.nvm/versions/node/v16.20.1*

방법
1. Homebrew의 Node.js로 바꾸기
   실행: `nvm use system`
2. 초기화 후(터미널을 재실행 시)에도 설정 유지하기
	1. 1번
	   실행 `nvm alias default node`
	2. 2번
		1. **Inspect Shell Initialization Files**: Open each of the relevant shell initialization files using a text editor (`nano`, `vim`, `emacs`, etc.) and search for any lines related to nvm or Node.js. Even if there are no explicit lines related to Node.js, there might be indirect configurations that affect the behavior.
		2. **Check Shell Configuration for All Users**: Sometimes, shell configurations might be present in system-wide initialization files (`/etc/profile`, `/etc/bashrc`, etc.) that affect all users. Check these files as well if you're making changes that should apply globally.
	3. 3번
		1. 실행: `env` 
		2. node.js 또는 nvm과 관련된 lines 찾기
			1. 저는 다음과 같은 결과가 있었습니다.
			   ```
			   MANPATH=/Users/tagg/.nvm/versions/node/v16.20.1/share/man:/opt/homebrew/share/man:: 
			   NVM_DIR=/Users/tagg/.nvm 
			   NVM_CD_FLAGS=-q 
			   NVM_BIN=/Users/tagg/.nvm/versions/node/v16.20.1/bin 
			   NVM_INC=/Users/tagg/.nvm/versions/node/v16.20.1/include/node
			   ```
	
		3. nvm 관련 환경 변수 설정 없애기
			1. 실행:
			   ```
			   unset NVVM_DIR
			   unset NVM_CD_FLAGS 
			   unset NVM_BIN 
			   unset NVM_INC
			   ```
		4. 다시 `env`를 실행하여 확인했더니 앞서 보았던 NVM 관련 lines가 사라졌습니다.


##### Reference
- [javascript - How do I completely uninstall Node.js, and reinstall from beginning (Mac OS X) - Stack Overflow](https://stackoverflow.com/questions/11177954/how-do-i-completely-uninstall-node-js-and-reinstall-from-beginning-mac-os-x)


#### Change default version
##### NVM
1. 설치된 node.js 버전 확인하기
   run: `nvm ls` 
2. 특정 버전 사용 설정하기
   run: `nvm use <version>`
3. 적용됐는지 확인하기
   run: `node -v`
4. 새로운 shell에서도 설정 유지하기
   run: `nvm alias default <version>`