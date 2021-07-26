깃에서 hexo 설치 방법

1. brew install node
2. npm install -g hexo-cli
----------------------------
참고사항
1. brew는 homebrew를 다운받아야 사용할 수 있다. 따라서 
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"를 터미널에 붙여넣는다. (Homebrew사이트에서 복사 가능)

2. brew에서 node를 설치하는 것이 아니라 node.js 홈페이지에서 node를 다운받을 경우 2번 명령어입력 시 권한 에러가 뜬다. 이럴경우 sudo/root를 사용해서 설치가 가능하지만 hexo 공식 문서에는 권장하지 않는 방식이다. 따라서 반드시 brew로 설치한다.

3. 만약 brew를 통해 설치하지 않을 경우 brew로 재설치를 해도 계속 권한 오류가 발생한다. 이럴 때는 nvm, npm, node를 전부 삭제한 후 재설치를 한다.

4. brew로 재설치하는데 The `brew link` step did not complete successfully라는 에러가 발생하는 경우가 있다. 이 때 brew link --overwrite node 명령어를 입력한 후 brew reinstall node 를 입력할 셩우 정상적으로 설치가 되는 것을 확인할 수 있다.

5. 버전확인 방법
● npm 버전 확인 방법: npm -v
● node 버전 확인 방법: node -v
● nvm 버전 확인 방법: nvm --version
● git 버전 확인 방법: git --version
● hexo 버전 확인 방법: hexo -v
