Backtick βοΈ
=============
Fanxy strings β
-------------

### What is backtick(``)? π¬
#### Template literals π₯
+ λ°±ν± μμμλ white-space(λμ΄μ°κΈ°, μ€λ°κΏ λ±) κ° λͺ¨λ μ μ©λλ€. 
+ Expression interpolation(ννμ μ½μ) μ΄ κ°λ₯ν¨
```java
console.log(`i'm ${22+2} years old`)
// output -> i'm 24 years old
```
+ Tagged templates μ μ΄μ©νμ¬ ν¨μλ₯Ό νμ±ν  μ μμ
```java
const name = "geon";
console.log(`hi my name is ${name}`)
// output -> hi my name is geon
```
+ HTML Fragments
```java
 template: `
    <div>
      <h1>My Component</h1>
      <p>back-tick is useful</p>
    </div>
  `
 // μλ°μ€ν¬λ¦½νΈμμ html νκ·Έλ₯Ό μ¬μ© κ°λ₯
```
### Others π¬
#### includes, repeat, startwith, endwith π₯
+ includes
 ```java
 const isEmail = (email) => email.includes("@");
 console.log(isEmail("phgst12@gmail.com"));
// output -> true
```
+ repeat
 ```java
 console.log("*".repeat(10))
// output -> ********** (λΉμ°νμ§λ§ string typeλ§ κ°λ₯)
```
+ startwith, endwith
```java
const name = "doctor.strange";

console.log(name.startsWith("doctor"));
console.log(name.endsWith("strange"));
// output -> true
// output -> true
```
<hr> </hr>



### SUM π€   
#### String μ λ³΄λ€ νΈνκ² μ¬μ© κ°λ₯ν μ¬λ¬ λ°©λ²λ€   
+ "" + "" + ν¨μ X   
=> (λ°±ν±)string string ${ν¨μ}(λ°±ν±) O
 
