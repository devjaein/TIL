## 어노테이션(REST API)

+ @RequiredArgsConstructor : final이 붙거나 @NotNull이 붙은 생성자를 자동 생성해주는 롬복 어노테이션, 생성자 주입을 할 때 만들기 번거로운 생성자를 만들어줌으로써 코드를 깔끔하게 만들 수 있음

+ @GetMapping : Get방식으로 URI가 요청된 경우 매핑되는 어노테이션, 조회할 때 사용

+ @PostMapping : Post방식으로 URI가 요청된 경우 매핑되는 어노테이션, 값을 넣을 때 사용

+ @PatchMapping : Patch방식으로 URI가 요청된 경우 매핑되는 어노테이션, 값의 일부를 수정하고 싶을 때 사용

+ @PutMapping : Put방식으로 URI가 요청된 경우 매핑되는 어노테이션, 값을 전부 수정하고 싶을 때 사용

+ @DeleteMapping : Delete방식으로 URI가 요청된 경우 매핑되는 어노테이션, 값을 삭제할 때 사용

+ @RequestParam : 파라미터로 입력 받을 때 사용하지만 사용하지 않아도 파라미터로 입력을 받음, 명시적으로 사용하는 경우가 있음

+ @RequestBody : json 형태로 데이터를 받고 싶을 경우 사용

+ @PathVariable : URI 주소에 동적으로 매핑되는 값이 있을 때 매서드의 파라미터에 @PathVariable를 사용
