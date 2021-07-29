conflict의 해결방법
상황: 협업을 진행하다보면 충돌이 발생할 수 있다.
먼저 깃허브에서 팀장의 git 주소를 git clone을 할 경우 작업 공간이 같아 협업 시 불편함을 가지고 있다. 깃허브는 이러한 문제점을 해결하기 위해 fork라는 기능을 사용하여 사용자 자신의 주소를 만들 수가 있다. fork를 해서 만든 깃허브에 자신의 주소를 가져와 git clone를 진행한다.
상황1: 새로운 브랜치를 만드는데 이때 git flow init()을 하여 새로 생성된 브랜치에서 진행을한다.
상황2: git flow feature start [새 브랜치명]을 작성하고 파일 수정 및 커밋을 한 다음 git flow feature finish[새 프랜치명]을 입력한다.
상황3: push를 진행하는데 원격에서 merge된 파일과 충돌이 발생한다.

해결방법: 1. 먼저 원격에 수정된 변경사항을 로컬로 최신화시킨다.
명령어: 1-1. git remote add upstream[원래 깃허브의 URL] -> git fetch upstream develop -> git merge FETCH_HEAD
        1-2. git remote add upstream[원래 깃허브의 URL] -> git pull upstream develop
2. 로컬의 파일들이 원격과 동일하게 최신화되어있을 것이다.
3. 파일 수정, add, commit를 한다.
4. git push origin develop (처음에 한번 push를 해서 conflict가 발생했기 때문에 git push -u origin develop를 하지 않아도 된다.) 
