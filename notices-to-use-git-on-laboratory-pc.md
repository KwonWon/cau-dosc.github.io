# 공용PC에서 Git 사용 시 주의사항

## 1. user.name, user.email 등록 시
 
저장소안으로이동후 `git config --local`로 해당 저장소 안에 설정 저장

```sh
$ cd <my_local_repo>
$ git config --local user.name <your name>
$ git config --local user.email <your email>
```

## 2. git push 실패 시 (permission denied)

- ### GitHub 프로젝트에 콜라보레이터로 추가되어 있는지 확인

  [콜라보레이터 추가 방법](github-for-newbie.html#4-콜라보레이터-추가)

- ### 작성자/이메일 확인

  1. git commit의 작성자/이메일이 GitHub 계정에 등록한 이름과 이메일이 일치하는지 확인
  2. 일치하지 않을 경우 `git commit --amend --author="yourname <youremail>"` 혹은 `git config` 설정 후 `git commit --amend --reset-author`로 commit 수정

- ### 인증 확인

  git remote 주소 확인 방법 `git remote -v`

  #### https 인증 확인 (git remote 주소가 "http://"로 시작할 경우)

  https 인증 시에 git push 명령어 실행 시 ID/PASSWORD 입력을 요구하지 않을 경우 확인 (Windows)
   - 윈도우에서 "자격 증명 관리자" 검색하여 프로그램 열기
   - "일반 자격 증명" 항목에서 GitHub 관련 자격증명 삭제 후 재시도

  #### ssh 인증 확인 (git remote 주소가 "git@github.com:" 로 시작할 경우)

   - [Conneting to Github with SSH](https://help.github.com/articles/connecting-to-github-with-ssh/)
     > 영문, GitHub 공식문서
   - [GitHub SSH 키 생성 및 등록하여 사용하기](http://nickjoit.tistory.com/94)
     > 국문, 블로그

## 3. Git 설치 시 주의사항

 * Enable Git Credential Manager 체크박스 해제

![](images/image.png)
