# GitHub 사용 가이드

## 1. 회원가입

1. [https://github.com/](https://github.com/) 접속
2. Username, Email, Password 입력 후 `Sign up for GitHub` 클릭

   ![](images/sign-up-for-github.PNG)

## 2. 프로젝트 생성

1. 화면 우측 ![](images/new-repository-button.PNG) 클릭
2. `Owner` 확인 후 `Repository name`에 프로젝트 이름 기입 후 `Create repository` 클릭

   ![](images/create-new-repository.PNG)

## 3. 소스코드 올리기

### 저장소에 올릴 `git commit`이 없는 경우

아래 스크린샷의 명령어 실행. 단, `git remote add` 명령어에서 "https://"로 시작하는 주소를 자신이 생성한 저장소로 설정

   ![](images/empty-repo-create-a-new-on-the-command-line.PNG)


### 저장소에 올릴 `git commit`이 이미 있는 경우

1. 프로젝트 메인 페이지의 Quick setup 항목에서 HTTPS 클릭하여 `https://`로 시작하는 주소 복사

   ![](images/empty-repo-quick-setup.PNG)

2. `git remote add origin <주소>` 명령어로 주소(https://...) 추가
3. `git push -u origin master` 명령어로 현재 commit 푸시 ([`git push` 실패 시 체크리스트](notices-to-use-git-on-laboratory-pc.html#2-git-push-실패-시-permission-denied))

   ![](images/empty-repo-push-a-existing-repo.PNG)

## 4. 콜라보레이터 추가

저장소를 만든 사람이 아닌 다른 사람이 `git push`를 하기 위해서는 프로젝트에 push 권한이 있어야 합니다.

1. 프로젝트 메인 페이지에서 `Settings` 클릭
2. 왼쪽 항목 중 `Collaborators` 클릭
3. 콜라보레이터 입력창에 아이디 혹은 이메일 주소 입력하여 추가

   ![](images/settings-collaborator.PNG)
