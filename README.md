# 문자열 덧셈 계산기

### 기능 요구 사항
입력한 문자열에서 숫자를 추출하여 더하는 계산기를 구현한다.

- 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환한다.
  - 예: "" => 0, "1,2" => 3, "1,2,3" => 6, "1,2:3" => 6
- 앞의 기본 구분자(쉼표, 콜론) 외에 커스텀 구분자를 지정할 수 있다. 커스텀 구분자는 문자열 앞부분의 "//"와 "\n" 사이에 위치하는 문자를 커스텀 구분자로 사용한다.
  - 예를 들어 "//;\n1;2;3"과 같이 값을 입력할 경우 커스텀 구분자는 세미콜론(;)이며, 결과 값은 6이 반환되어야 한다.
- 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.

### 기능 목록
- 문자열 입력
- 커스텀 구분자 추가 기능
- 입력 받은 문자열(, : custom)을 기반으로 값 반환
- 예외 처리
  - //를 입력하고 뒤에 \n을 입력하지 않은 경우 ✅
  - 처음부터 //나 숫자가 아닌 임의 값을 넣은 경우 ✅
  - 커스텀 구분자를 사용하지 않고 숫자 사이에 임의 값을 넣은 경우 ✅
  - 커스텀 구분자를 사용하고 중간에 아무것도 안넣은 경우 ✅
  - 올바르지 않은 수식인 경우 ex) ,1, ✅
  - 음수가 들어오는 경우 ✅
  - custom 문자열이 , : 인 경우 ✅

### 공부 할 것
- Java 8, 11, 17, 21의 차이점
- 자바 문자열 관련 학습 
