var vs let, const
=============
Block Scope
-------------

### what is Block Scope?  π¬
+ scope = λ²μ
+ block μ νμμ {}(μ€κ΄νΈ) λ‘ κ΅¬μ±λμ΄ μμ
+ block scope λ μ ν¨λ²μκ° {}(block) μ΄λΌλ μλ―Έ 
+ block scope μ κ²½μ° block λ°μμ μμ κ²μ μ¬μ©νμ§ λͺ»νμ§λ§ μμμ  λ°μ κ²μ μ¬μ©ν  μ μμ   
=> const, let = block scope   
=> var = function scope (function λ΄ var μ μ μΈ ν block μλ μ κ·Όμ΄ κ°λ₯)   
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
 
