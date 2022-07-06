Dead Zone
=============
hoisting
-------------

### var vs let 💬
자바스크립트는 호이스팅이라는 특징을 가지고 있는데, 소스코드를 순서대로 런타임 하기 이전 변수 선언을 먼저 함.   
하지만 let 호이스팅을 막고 소스코드 순서대로 실행됨   
+ var 은 소스코드 순서와 상관없이 어디에서든 위치할 수 있고 이로 인해 실수를 유발할 수 있음
+ 그러나 let 에는 temporal dead zone 이라는 것이 있는데, 이것이 호이스팅을 막고 소스코드 순서대로만 실행되도록함

 <hr/>
 
 
 ### SUM
 #### so, use let!!

var = hoisting   
let = no hoisting   

 
