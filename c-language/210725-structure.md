구조체

구조체는 여러개의 변수를 묶어 하나의 객체를 표현하고자 할 때 사용합니다.
구조체는 변수에 접근할 때 .(온점)을 사용합니다.

사용방법
structure person{
   int age;
   int name;
};

int main(void){
   struct person p1;

   p1.age = 26;
   p1.name = 홍길동;
}

포인터로 사용할 경우에는 .(온점)대신 ->를 사용합니다.

structure person{
   int age;
   int name;
}

int main(void){
   struct person *p;

   p1 -> age = 26;
   p1 -> name = 홍길동;
}
