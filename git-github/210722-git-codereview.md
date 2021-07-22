코드리뷰하는 방법
1. 새로운 branch를 생성(git branch 새로운 브랜치명)
2. 새로 생성한 branch가 맞는지 확인하고 아니라면 새로 생성한 branch에 파일이 생성되도록 설정(git status, git switch 새로운 branch)
3. 파일 생성(touch)
4. 깃허브에 push(add, commit, push)
5. 깃허브에 Setting에 들어가 Manage access에 코드리뷰해줄 관리자의 username를 적는다.
6. 관리자가 승인하면 관리자가 코드리뷰를 할 수 있다.
7. 코드리뷰 받는 사람: pull reㅏquests를 -> new pull requests -> [base : main <- compare : 새브랜치](확인) -> review -> 글 작성 -> create pull request
8. 코드리뷰 하는 사람: 메일에 들어가 확인 -> 주소 입력 -> pull request -> 소스에 +를 눌러 리뷰 작성 -> Finish your review
9. 깃에서 수정하여 다시 push -> pull request -> refresh -> merge pull request(main 브랜치에 등록)
