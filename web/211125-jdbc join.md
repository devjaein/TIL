## jdbc join

#### 웹 프로그래밍 개발시 join테이블을 세션에 저장해 불러오는 방법
테이블을 조인하면 vo에는 없는 객체를 필요로하게 된다.  
이때 기존의 방식대로 사용하게되면 해당 객체를 찾을 수 없어 오류가 발생한다.  
해결하는 방법은 두가지가 있다.  
+ 조인한 테이블에서 사용하는 vo를 새로 만든다.
+ map을 사용해 vo를 사용하지 않고 저장한다.
 첫번째 방법은 계속적으로 사용할 경우에 사용하는 것이 좋다.  
 하지만 만약 한번만 사용하는 경우라면 두번째가 편하며 공간을 덜 차지한다는 장점을 가지고 있다.  
 
###### 예제
``` java
public List<Map<String, String>> getBlogList(BlogVO vo) {
		List<Map<String, String>> blogList = new ArrayList<Map<String,String>>();
		try {
    .
    .
    .
    }
    catch (Exception e) {
    ...
    } finally {
    ...
    }
    return blogList;
}
```
