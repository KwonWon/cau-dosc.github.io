### user.name, user.email 등록 시
 
저장소안으로이동후 git config --local로 해당 저장소 안에 설정 저장

```sh
$ cd <my_local_repo>
$ git config --local user.name <your name>
$ git config --local user.email <your email>
```

- - -

### git push 실패 시 (permission denied)

1. GitHub 상에서 프로젝트에 Push 권한이 있는지 확인
2. git remote 주소 확인 `git remote -v`

#### 주소가 "https://" 로 시작할 경우 (Windows의 경우)

 - 윈도우에서 "자격 증명 관리" 검색하여 프로그램 열기
 - github 관련 자격증명 삭제 후 재시도

* 스크린샷 포함한 상세한 내용 추가 예정

#### 주소가 "git@github.com:" 로 시작할 경우

 아래 URL 항목 참고

 - https://help.github.com/articles/connecting-to-github-with-ssh/ (영문, GitHub 공식문서)
 - http://nickjoit.tistory.com/94 (국문, 블로그 "GitHub SSH 키 생성 및 등록하여 사용하기")

- - -


### 설치 시 주의사항

 * Enable Git Credential Manager 체크박스 해제

![](images/image.png)
