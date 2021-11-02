## JadenCase 문자열 만들기

#### 문제
https://programmers.co.kr/learn/courses/30/lessons/12951

#### 풀이
``` python3
def solution(s):
    result = []
    s = s.lower()
    for i in s.split(" "):
        if i == '':
            pass
        if i[0].isalpha():
            result.append(i[0].upper() + i[1:])
        else:
            result.append(i)

    return " ".join(result)
```

#### 정답
``` python3
def solution(s):
    s=s.split(' ')
    for i in range(len(s)):
        s[i]=s[i][:1].upper() + s[i][1:].lower()
    return ' '.join(s)
```

#### 회고
1. 문제 자체는 어렵지 않았지만 테스트케이스에서 계속해서 런타입 에러가 발생했다. 공백이 2개일때 처리를 해주지 않아 발생하는 문제였다.(ex ^^aa ^^bb일 경우 Aa Bb가 되야함)

#### 풀이(JAVA)
``` java
class Solution {
    public class solution(String s) {
        answer = '';
        String[] sp = s.toLowerCase().split("");
        boolean flag = true;
        
        for(String ss : sp) {
            answer += flag ? ss.toUpperCase() : ss;
            flag = ss.equals(" ") ? true : false;
        }
    }
}
```
