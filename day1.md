# 우테캠 day1

## 오전

- 우아한형제들 큰집 투어
- 김범준 대표님 환영사

## 점심

- 첫 날 특별 도시락 제공!

## 오후

- 아이스브레이킹 (빙고)

### 소개

- [테크캠프 가이드](https://docs.google.com/document/d/1SNS4F4IvQFn_Z8mjvU2NIH-5DB_hlbCWAWc6ScrS7Ps/edit#)

- 환경설정

- 테크캠프에 임하는 각오

  > 우아하게 코딩하는 우아한 사람이 되자 😇

### Git, GitHub 

- 깃헙 프로젝트 수행 with 최해랑님



- **Git** : 소스 코드 버전 관리 및 협업을 위해 사용하는 VCS (Version Control System)
  - working directory - stage (`add`) - local storage (`commit`) - remote storage (`push`)
  - **commit**
    - **깃에 실제로 존재하는 것은 커밋밖에 없다**
    - tree 로 구성되고, 각각의 커밋은 이전 커밋을 가리키고 있다.
    - **커밋은 영구적으로 저장됨 (`reset` 을 하더라도 로컬저장소 어딘가에는 남아있다!)**
      - *아래 내용 다시 확인/실습할 것*
      - ~~`git branch test [날린 커밋의 체크섬]` - `git checkout test`~~
      - ~~`git reflog` : 작업했던 모든 체크섬의 기록 확인 가능~~
    - **커밋을 하더라도 스테이지의 내용은 그대로 남아있다**
      - *아래 내용 다시 확인할 것*
      - ~~커밋할 내용이 없다는 것의 의미는 WD 와 HEAD 의 내용이 동일하다는 의미?~~
      - ~~커밋할 변경 사항: wd와 stage 는 내용이 같고 Head 커밋하고는 다르다~~
    - 브랜치는 어떤 내용을 담고 있는 것이 아니라 커밋에 대한 **참조**
    - **깃은 diff 가 아니라 파일을 통채로 저장한다**
      - 특정 커밋으로 checkout 하는 경우에 큰 장점이 됨
      - 파일 내용이 동일하다면 그 파일을 참조하는 방식으로 파일을 저장하기 때문에 동일한 파일은 하나만 존재하게 된다.
      - 과거 유물이 되고 있는 svm 은 diff를 저장하기 때문에 처음 커밋부터 특정 시점(checkout)까지를 만들어내어야 했다.
- **Github** : Git을 호스팅해주는 사이트, 소셜코딩
- Git 기본 명령어
  - `git init`
    - 로컬저장소 (.git) 생성
  - `git clone [원격저장소 주소]`
  - `git add [파일명]`, `git commit`, `git push [원격저장소명] [원격저장소 브랜치명]`, `git pull [원격저장소명] [원격저장소 브랜치명]`
  - `git branch [브랜치명]`, `git checkout [브랜치명]`, `git merge [브랜치명]`
    - *아래 내용 다시 확인/실습하기*
    - ~~merge 하면 자동으로 커밋이 하나 더 생성됨~~
    - ~~`git rebase master` > `git merge` : 커밋 정리 가능~~
- GitHub 기본 기능
  - pull request
  - fork : 권한이 없는 레포에 pull request 할 때 활용
- 조심할 부분
  - ~~git flow~~ > github flow
  - ~~`git add .`~~ > `git add [파일명]`
    - 하나의 기능 단위로 자주 커밋할 것 (하나의 함수 정도)
    - 한편, 풀리퀘는 해당 브랜치를 만든 목적 (ex. login) 이 달성되었을 때 보내는 것이 일반적
  - ~~`git commit -m [커밋메세지]`~~ > `git commit` 후  editor 에서 자세히 작성할 것

### 개별적으로 확인할 내용

추가 학습할 내용 *(feat. Do it! 지옥에서 온 문서관리자 깃&깃허브 입문)*

- tag
- reset
- rebase
- revert
- stash
- fetch
- `git hash-object [파일명]` : 해당 파일의 체크섬 확인
- `git ls-files --stage` : 스테이지의 내용 보기
- `tree .git`
- `git cat-file -t ce013`



## 참고자료

- [git visualization](https://learngitbranching.js.org/?locale=ko)

- [터미널 꾸미기](https://nolboo.kim/blog/2015/08/21/oh-my-zsh/)



## 하루의 끝.

싸피에서 배웠던 깃, 깃허브 관련 기본 내용을 복습했던 하루. `git reset` 으로 날린 커밋도 로컬저장소에 살아있고 되살릴 수도 있다는 내용은 새로운 꿀팁! 오랜만에 바깥 생활을 오래했더니 피곤해서 퇴근 후 침대에 누워있었지만 그래도 하루가 끝나기 전에 다시 한 번 열어보고 정리했다는 점에 뿌듯! 빠이팅!