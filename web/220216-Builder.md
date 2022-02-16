## Builder
빌더 패턴을 사용하는 이유는 첫째. 필요한 데이터만 설정, 둘째. 유연성 확보, 셋째 가독성을 높임, 셋째. 불변성을 확보할 수 있다는 장점들을 가지고 있기 때문이다.

#### 사용 방법
``` java
@Getter
@Builder
@Entity
public class User {
  @Id
  @GenerateValue
  private Long id;
  
  private String name;
  
  private String userId;
  
  private String password;
}
```
``` java
User user = User.builder()
              .id(3)
              .name("홍길동")
              .userId("develop")
              .password("asdasdasd")
              .build;
```
다음과 같이 @Builder을 사용함으로써 사용이 가능하며 사용하려는 값을 이런식으로 넣어준다.
만약 사용하지 않을 경우에는 entity(domain)에 @Setter을 추가해야하며 다음과 같은 방식으로 사용을 해야한다.
``` java
User user = new User();
user.setId(3L);
user.setName("홍길동");
user.setUserId("develop");
user.setPassword("asdasdasd");
```
