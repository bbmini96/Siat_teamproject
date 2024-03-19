### Git & Github 충돌 시나리오
Git과 Github를 사용하면서 발생할 수 있는 충돌 시나리오를 작성한 곳 입니다. \
많은 시나리오가 있겠지만 작은 예시 3개만 작성하였습니다.
<br><br>
#### 1. 같은 branch에서 같은 파일을 수정하는 경우
 - 희: test1.html을 수정 후 commit & push
 - 성: git pull을 하지 않고 test1.html을 수정 후 commit & push
    - Error? 
  
    - Why?

<br><br>
#### 2. 다른 Branch에서 같은 파일을 수정하는 경우
 - 창: test/changmin branch 생성 후 checkout
 - 희: test/huigwon branch 생성 후 checkout
 - 창: test2.html을 수정 후 commit & push
 - 창: main <- test/changmin merge
 - 희: git pull을 안 한 상태에서 test2.html을 수정 후 commit & push
 - 희: main <- test/huigwon merge
    - Error?

    - Why?

<br><br>
#### 3. Fork를 뜬 Repository에서 파일을 수정한 경우
 - 성: Siat_teamprojrct를 개인 Repository에 Fork
 - 창: test3.html 수정 후 commit & push
 - 성: git pull을 안 한 상태에서 test3.html을 수정 후 commit & push
 - 성: 창민님이 Oner인 Siat_teamprojrct에 PR
 - 창: PR 수락
    - Error?

    - Why?