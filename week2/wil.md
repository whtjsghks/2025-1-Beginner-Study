# 개발 입문 스터디 2주차 WIL

GitHub의 Fork / Star
-------------------

+ Fork: 다른 사용자의 레포지토리를 긁어올 수 있음
+ Star: 북마크와 같이 달아서 저장 가능

Branch & Merge
---------------

Issue, Pull request, Branch를 가장 많이 사용한다

+ Issue
    + 여러 기능들 task를 쪼개서 Issue로 등록
+ Branch
    + Issue를 분리된 공간에서 작업 후 merge 하는데, 분리를 가능하게 하는 것이다
    + fork와 다르게 같은 레포지토리에 생성된다
    + Branch Naming Convention
        + "type\<issue 번호(#~~)>-<간략한 설명>"
+ Pull Request
    + 분기된 branch를 다시 병합하기 위한 절차
    + merge에 앞서 코드 리뷰 필요 (lgtm : looks good to me)


### Merge의 3가지 옵션
+ Create a merge commit
    + 두 branch를 공통 부모로 하는 새로운 commit 'E'를 만듦
+ Squash and merge
    + A,B,C commit을 'squahs' 하나로 뭉텅이가 된다
    + 하나의 커밋으로 main 브랜치로 병합
+ Rebase and Merge
    + 당분간은 쓸 일이 없을 것
    + 커밋의 base를 재설정 -> 모두 새로운 커밋으로 변경
    + 주의! Commit hash가 변경됨 -> 무수한 충돌 발생 가능
        * Commit hash := Commit ID -> 커밋의 식별을 위해 사용하는 40자 길이의 16진수
    + 웬만하면 사용하지 않는 것이 좋다

https://github.com/whtjsghks/2025-1-Beginner-Study/pull/2