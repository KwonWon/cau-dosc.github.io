# GitHub에 올라온 커밋 합치기

## `git status`로 커밋을 합칠 수 있는 상태인지 확인하기

커밋을 합치기 위해서는 추적 중인 모든  파일이 Unmodified 상태이어야 합니다. 즉, 현재 수정 중인 내용이 있으면 commit으로 작성하여서, `git status`로 확인하였을 때 아래 스크린샷처럼 `nothing to commit, working tree clean` 메시지가 나오거나 `nothing to added to commit but untracked files present` 메시지가 나와야 합니다. ([File Status Lifecycle 참고](https://git-scm.com/book/ko/v1/Git%EC%9D%98-%EA%B8%B0%EC%B4%88-%EC%88%98%EC%A0%95%ED%95%98%EA%B3%A0-%EC%A0%80%EC%9E%A5%EC%86%8C%EC%97%90-%EC%A0%80%EC%9E%A5%ED%95%98%EA%B8%B0))

![](images/git-status-up-to-date-and-working-tree-clean.PNG)

## `git remote update` 명령어로 GitHub 저장소를 다운로드

![](images/git-remote-update.PNG)

## `git status` 명령어로 합칠 커밋이 있는지 확인

TBA

![](images/git-status-the-branch-is-ahead.PNG)
![](images/git-status-the-branch-is-behind.PNG)
![](images/git-status-the-branch-have-diverged.PNG)
