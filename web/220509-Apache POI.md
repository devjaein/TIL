## Excel 암호화

+ XSSF(Excel 2007 이상): 읽기와 쓰기가 가능하며 메모리 Flush 기능이 없어서 대용량 다운 불가능
+ + HSSF(Excel 2003 이하): XSSF와 기능 동일
+ SXSSF: 쓰기만 가능하며 메모리 Flush 기능 추가로 대용량도 문제 없음

##### 암호화 순서
템플릿 읽기 -> xssf읽기 -> sxssf로 변환 -> sxssf로 엑셀 작성 -> xssf로 변환(sxssf를 inputStream에 담아서 xssf를 inputstream으로 생성) -> xssf를 암호화(sxssf는 쓰기 전용이므로 읽어서 암호를 입히는 것은 불가능) -> xssf를 다운로드
