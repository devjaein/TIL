## Iterator

Collection 인터페이스에 iterator()메서드로 선언되어있으며 컬렉션에 저장된 요소들을 읽어오는 방법을 표준화한 것이다.  

#### 메서드
+ boolean hasNext(): 읽어올 요소가 있는지 확인
+ Object next(): 다음 요소을 읽어온다. next()를 호출하기 전에 hasNext()를 호출해서 읽어 올 요소가 있는지 확인하는 것이 안전
+ void remove(): next()로 읽어 온 요소를 삭제한다. next()를 호출한 다음에 remove()를 호출(선택적 가능)

#### 예제
``` java
import java.util.*;

public class Iterator {
    public static void main(String[] args) {
        ArrayList list = new ArrayList();
        list.add("1");
        list.add("2");
        list.add("3");
        list.add("4");
        list.add("5");

        java.util.Iterator it = list.iterator();

        while (it.hasNext()) {
            Object obj = it.next();
            System.out.println(obj);
        }
    }
}

```
