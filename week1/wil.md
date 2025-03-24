개발 입문 스터디 1주차
=====================

Git은 무엇인가
--------------

+ 버전 관리 및 협업을 위해 사용하는 오픈소스 소프트웨어

Git을 쓰는 이유
--------------

+ 누가, 언제, 어떻게 코드를 수정했는지 확인하기 위해

Git 파일의 생명주기
------------------

+ Untracked

+ Tracked
    + Unmodified
    + Modified
    + Staged

* * *

* Git의 영역
    + Working Directory
    + Staging Area
    + Repository

## 기본 명령어

+ 디렉토리에 Git 저장소를 만들기
  + git init
+ Git으로 관리할 대상 등록하기
  + git add
    + git add . : 모든 파일 한 번에 등록
    + git add "파일명" : 하나씩 등록
    + git rm --cached "파일명" : unstage로 되돌리기
+ 파일 수정 후 로컬 저장소로 옮기기
  + git commit

## Commit Message

+ "type : subject"

    + 새로운 기능을 추가한 경우
        + feat
    + 기존 코드를 개선한 경우
        + refactor
    + 버그를 수정한 경우
        + fix
    + 코드 외의 설정을 바꾼 경우
        + chore
    + 문서화
        + docs
    + 테스트 코드
        + test

+ Git에 커밋하기
    + git commit -m "commit message"

## GitHub에 올리기

+ GitHub에 있는 레포지토리와 Local 레포지토리 연결
    + git remote add origin <주소>
    + git branch -M main
    + git push -u origin main

+ GitHub에 올리기
    + git add <파일명>
    + git commit -m "commit message"
    + git push origin main