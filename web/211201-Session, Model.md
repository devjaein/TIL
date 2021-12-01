## Session과 Model
#### Session.setAttribute(), Model.addAttribute()

Session과 Model을 통해 데이터를 전송해 view에서 사용이 가능 하지만 둘은 어떻게 사용되는지 다름

+ Session은 WAS(톰캣)에서 관리, 전역 변수 같은 의미
+ Model은 MVC 패턴으로 컨트롤러는 DB에서 데이터를 가져와 Model에 담는다. View는 Model에 있는 데이터를 적절하게 사용
