## HashSet

HashSet는 Set의 성질과 같아 서로 중복되는 값이 들어올 수 없으며 순서는 상관이 없다.  
HashSet은 해싱을 이용해 구현되었기 때문에 붙여진 것이다.  
만약 HashSet에서 저장순서를 유지하고 싶다면 LinkedHashSet를 사용하면된다.  

#### Ex1
``` java
public class HashSetEx1 {
    public static void main(String[] args) {
        Object[] objArr = {"1", new Integer(1), "2", "2", "3", "3", "4", "4", "4"};
        Set set = new HashSet();

        for (int i = 0; i < objArr.length; i++) {
            set.add(objArr[i]);
        }

        System.out.println(set);
    }
}
```

#### Ex2
``` java
public class HashSetEx1 {
    public static void main(String[] args) {
        for (int i = 0; set.size() < 6; i++) {
            int num = (int) (Math.random() * 45) + 1;
            set.add(new Integer(num));
        }

        List list = new LinkedList(set);
        Collections.sort(list);
        System.out.println(list);
    }
}

```
