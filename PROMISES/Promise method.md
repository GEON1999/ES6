Promise methods βοΈ
=============
.all, .race, .finally β
-------------

### .all π¬
#### λ€μμ promise μ»¨νΈλ‘€ κ°λ₯ π₯
 ```java
const p1 = new Promise((resolve) => {
  setTimeout(resolve, 3000, "First");
});

const p2 = new Promise((resolve, reject) => {
  setTimeout(resolve, 2000, "second");
});

const p3 = new Promise((resolve) => {
  setTimeout(resolve, 1000, "third");
});

const motherPromise = Promise.all([p1, p2, p3]);

motherPromise
.then((value) => console.log(value))
.catch((err) => console.log(err));
// output ->Β ['First', 'second', 'third']
```
+ λ€μμ promise μ κ°μ λμμ μ¬μ©ν  μλ, κ·Έμ€ μ€λ₯κ° μλ promise κ° μλμ§ κ²μν  μλ μμ
+ λ¨Όμ  pending μ΄ λλ promise μμκ° μλ, Promise.all(1, 2, 3) μμ κΈ°μ¬λ μμλλ‘ κ°μ΄ λμ΄λ¨
 
 <br/>
 
 ### .race π¬
#### promise μ€ κ°μ₯ λ¨Όμ  pending μ΄ μλ£λ κ°μ μ΄ννκ±°λ κ±°λΆν¨ π₯
+ μμ
 ```java
const p1 = new Promise((resolve) => {
  setTimeout(resolve, 3000, "First");
});

const p2 = new Promise((resolve, reject) => {
  setTimeout(resolve, 2000, "second");
});

const p3 = new Promise((resolve) => {
  setTimeout(resolve, 1000, "third");
});

Promise.race([p1, p2, p3])
.then((value) => console.log(value))
.catch((err) => console.log(err));
// output -> third
```


 <br/>

### .finally π¬
#### promiseμ μ‘°κ±΄μ΄ μΆ©μ‘± μ¬λΆμ κ΄κ³ μμ΄ promise μ²λ¦¬κ° μλ£λλ©΄ λ¬΄μ‘°κ±΄ μ€νλλ μ½λ π₯
+ μμ
 ```java
const p1 = new Promise((resolve, reject) => {
  setTimeout(reject, 1000, "First");
})
.then((value) => console.log(value))
.catch((e) => console.log(`${e}error`))
.finally(() => console.log("Im done"));
// output -> Firsterror / Im done
```
+ error μ catch νκ³  μ½μμ°½μ μΆλ ₯νμμλ Im done μ μ½μμ°½μ μΆλ ₯ν¨

 <hr/>
 
 
 ### SUM π€
#### promiseμ λ€μν λ©μλ

 
