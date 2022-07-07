Backtick ✍️
=============
Fanxy strings ☑
-------------

### What is backtick(``)? 💬
#### Template literals 🔥
+ 백틱 안에서는 white-space(띄어쓰기, 줄바꿈 등) 가 모두 적용된다. 
+ Expression interpolation(표현식 삽입) 이 가능함
```java
console.log(`i'm ${22+2} years old`)
// output -> i'm 24 years old
```
+ Tagged templates 을 이용하여 함수를 파싱할 수 있음
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
 // 자바스크립트에서 html 태그를 사용 가능
```
### Others 💬
#### includes, repeat, startwith, endwith 🔥
+ includes
 ```java
 const isEmail = (email) => email.includes("@");
 console.log(isEmail("phgst12@gmail.com"));
// output -> true
```
+ repeat
 ```java
 console.log("*".repeat(10))
// output -> ********** (당연하지만 string type만 가능)
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



### SUM 🤝   
#### String 을 보다 편하게 사용 가능한 여러 방법들   
+ "" + "" + 함수 X   
=> (백틱)string string ${함수}(백틱) O
 
