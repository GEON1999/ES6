REST&SPREAD βοΈ
=============
... β
-------------

### Spread π¬
#### unpack π₯
+ μμ
 ```java
 const allowedForTeen = {
  pcCafe: true
 }
 
 const allowedForAdult = {
 ...allowedForTeen,
 alcohol: true
 }
 
 const allowedForOld = {
  ...allowedForAdult,
  kidsZone : "true"
 }
 
console.log("teen", allowedForTeen);
console.log("adult", allowedForAdult);
console.log("old", allowedForOld);
// output -> teen {pcCafe: true} / adult {pcCafe: true, alcohol: true} / old {pcCafe: true, alcohol: true, kidsZone: false}, 
```
+ μλμ κ°μ΄λ κ°λ₯ν¨
 ```java
 const allowedForAdult = {
  pcCafe: true,
  alcohol: true
 }
 
 const female = {
  womanRestroom : true
 }
 
 const allowedForFemaleAdult = {
  ...female,
  ...allowedForAdult
 }
console.log(allowedForFemaleAdult);
// output -> {womanRestroom: 'true', pcCafe: true, alcohol: true}
```
+ μ object μ κ°μ΄ array μμλ λμΌνκ² μ¬μ© κ°λ₯ν¨

<br/>

### REST π¬
#### λλ¨Έμ§ parameter π₯

```java
const user = {
  name: "nico",
  age: 24,
  password: 12345,
};

user["password"] = null;

console.log(user);
// output -> {name: 'nico', age: 24, password: null}

const killage = ({ age, ...rest }) => rest;

const cleanuser = killage(user);

console.log(cleanuser);
//output - > {name: 'nico', password: null}

const setCountry = ({ country = "KR", ...rest }) => ({ country, ...rest });

console.log(setCountry(user));
//output - > {country: 'KR', name: 'nico', age: 24, password: null}

const rename = ({ name: newname, ...rest }) => ({ newname, ...rest });

console.log(rename(user));
//output - > {newname: 'nico', age: 24, password: null}
```
+ λλ¨Έμ§ λ§€κ°λ³μλ₯Ό μ΄μ©νμ¬ λλ¨Έμ§ κ°λ§ λ°νν  μλ, μ€λΈμ νΈ μμ μλ key&value λ₯Ό μμ ν  μλ, μΆκ°ν  μλ μμ 

 

 <hr/>
 
 
 ### SUM π€
#### DESTRUCTURING + REST&SPREAD = π₯

 
