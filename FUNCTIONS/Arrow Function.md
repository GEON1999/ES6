Arrow Function βοΈ
=============

### What is Arrow function? π¬
#### λ³΄κΈ° νΈν ν¨μ π₯
+ arrow : =>
μμ )
```java
//before
names.map(function(item) {return item + ","};
// arrow function
names.map(item => {return item + ","});
// implicit return : whatever i put in same line, it will be returned.
names.map(item => item + ",");
// argument κ° 2κ° μ΄μμΈ κ²½μ° index νμ
names.map((item, index) => item + "," + index);
```

### This π¬
#### When we should no use arrow function π₯
+ arrow function μμ μλ thisλ window λ₯Ό μ°Έμ‘°ν¨   
- this λ₯Ό μ¬μ©νκ³  μΆλ€λ©΄ arrow function μ μ¬μ©ν΄μλ μλ¨

### Default values
#### property(argument)'s default value  π₯
```java
const hi = (name = "geon") => `hello ${name}`
console.log(hi());
// output -> 'hello geon'
// default value κ° μλ κ²½μ°μ undifiend
```
 

 <hr/>
 
 
 ### SUM π€
#### μ°κΈ°λ, λ³΄κΈ°λ μ¬μμ§ ν¨μ
+ this ν€μλ μ¬μ© μ arrow function μ¬μ© x
+ κ°μ μ€μμ  return νμ§ μμλλ¨ ({} μ¬μ© x)
+ κ°μ μ€μ΄ μλ κ²½μ°μ ({}) κ³Ό κ°μ΄ μ¬μ© μ return μλ΅ κ°λ₯
 
