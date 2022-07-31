VARIABLES
=============
const & let 💨
-------------

### 기존의 var 은 왜 사용하지 않는가? 💬
변수의 값을 변하지 않게 지킬 안정장치가 없음   
 => Semantic code 를 작성하기 위해 같은 의미에 같은 이름의 변수가 선언되면 그 값이 바뀌게 됨
 
### What is Const?
##### const is constant. 
 + const 로 선언한 변수의 값은 __바꿀 수 없음__   
 ex) 
 ```java
 const name = "geon";
 name = "haru";
 // output -> Error: "name" is read-only
 ```
 + 변수 자체는 변경되지 않지만, 변수의 값이 object 인 경우 변수 내 __object 의 값은 바꿀 수 있음__   
 ex)
 ```java
 const dog = {
  name: "haru"
 }
 dog.name = "ruby"
 // output -> dog.name = "ruby"
 ```
 + 추후 추가 안전장치 설정 방법 추가 예정
 
 ### What is Let?
 ##### it's just like var
 변수를 선언하고 값을 변경할 수 있음

---
 


 
 ### SUM
 안전하게 사용할 수 있는 const 를 통상적으로 사용하고, 변수의 값을 업데이트 해야하는 상황에서만 let 을 사용하는 것이 안전함 
 

 ---
 
 모던 자바스크립트 딥다이브를 읽으면서 const, let 에 대한 정리를 추가 했음 아래 참고   
 [__모던 자바스크립트 딥다이브__](https://github.com/GEON1999/Modern-JavaScript-Deep-Dive/blob/main/docs/Today%20I%20Learn%20(1%EB%B6%84%EA%B8%B0)/ch15_let%2C%20const%20%ED%82%A4%EC%9B%8C%EB%93%9C%EC%99%80%20%EB%B8%94%EB%A1%9D%20%EB%A0%88%EB%B2%A8%20%EC%8A%A4%EC%BD%94%ED%94%84/%ED%95%98%EB%A3%A8_TIL.md)
