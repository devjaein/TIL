## Comparator, Comporable

자바에서는 정렬을 할 때 주로 Charcter 클래스의 Comparable를 사용해 구현을 한다.  
Comporable는 작은 값에서부터 큰 값의 순으로 정렬되도록 구현되어있다.   

Comporator와 Comporable에는 Compare() 메서드와 CompareTo()메서드가 있다.
둘 다 객체를 비교하여 두 객체가 같으면 0, 비교하는 값보다 작으면 음수, 크면 양수를 반환한다.  

+ Comparable: 기본 정렬기준을 구현하는데 사용
+ Comparator: 기본 정렬기준 외에 다른 기준으로 정렬하고자할 때 사용
