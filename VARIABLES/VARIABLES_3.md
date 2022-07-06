var vs let, const
=============
Block Scope
-------------

### what is Block Scope?  💬
+ scope = 범위
+ block 은 한쌍의 {}(중괄호) 로 구성되어 있음
+ block scope 는 유효범위가 {}(block) 이라는 의미 
+ block scope 의 경우 block 밖에서 안에 것을 사용하진 못하지만 안에선 밖에 것을 사용할 수 있음   
=> const, let = block scope   
=> var = function scope (function 내 var 을 제외 한 block 에는 접근이 가능)   
ex)
 ```java
var x = 1;
let y = 1;

if (true) {
  var x = 2;
  let y = 2;
}

console.log(x);
// expected output: 2

console.log(y);
// expected output: 1
 ```
Link: [block MDN](https://google.com](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/block, "block mdn link")
 

 <hr/>
 
 
 ### SUM


not to make mistakes, always use const&let
 
