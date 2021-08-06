깃에서 커밋한 파일 취소하기

깃에서 커밋을 할 때 잘못 올렸거나 다시 내리고 싶은 경우가 발생할 때가 있다.  
이러한 문제를 해결하기 위한 방법이다.  
1. git log //commit 목록 확인  
2. git reset HEAD^ // 가장 마지막에 커밋한 커밋 취소  
2-1. git reset HEAD~2 // 마지막 2개의 commit를 취소  

참고  
add를 취소하는 방법
1. git status // 파일들의 상태 확인
2. git reser HEAD [file] //Unstage로 변경 
