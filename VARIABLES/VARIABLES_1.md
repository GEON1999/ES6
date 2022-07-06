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
 <hr/>
 
 
 ### SUM
 안전하게 사용할 수 있는 const 를 통상적으로 사용하고, 변수의 값을 업데이트 해야하는 상황에서만 let 을 사용하는 것이 안전함 
 
