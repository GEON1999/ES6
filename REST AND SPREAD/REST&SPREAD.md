REST&SPREAD ✍️
=============
... ☑
-------------

### Spread 💬
#### unpack 🔥
+ 예시
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
+ 아래와 같이도 가능함
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
+ 위 object 와 같이 array 에서도 동일하게 사용 가능함

<br/>

### REST 💬
#### 나머지 parameter 🔥

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
+ 나머지 매개변수를 이용하여 나머지 값만 반환할 수도, 오브젝트 안에 있는 key&value 를 수정할 수도, 추가할 수도 있음 

 

 <hr/>
 
 
 ### SUM 🤝
#### DESTRUCTURING + REST&SPREAD = 💥

 
