## 레이어 별 어노테이션 설정

+ @Service : ...ServiceImpl - 비즈니스 로직을 처리하는 Service 클래스
+ @Repository : ...DAO - 데이터베이스 연동을 처리하는 DAO 클래스
+ @Controller : ...Controller - 사용자 요청을 제어하는 Controller 클래스

해당 3개의 어노테이션은 전부 @Component 어노테이션을 가지고 있으므로 컴포넌트 스캔의 대상이된다.
