Promises Chaining ✍️
=============
2nd header(opt) ☑
-------------

### 주제 💬
#### 요약 🔥

![프로미스 체이닝](https://cdn.discordapp.com/attachments/446295737454821404/995509806808961084/unknown.png)

+ 예시
 ```java
const amIdouble = new Promise((resolve, reject) => {
resolve(2);
});

const timesTwo = (numbertwo) => numbertwo * 2;

amIdouble
.then(timesTwo)
.then(timesTwo)
.then(timesTwo)
.then(timesTwo)
//.then(() => {
// throw Error("something is wrong");})
.then((lastNumber) => console.log(lastNumber))
//.catch((error) => console.log(error));
// output -> 32
```

 

 <hr/>
 
 
 ### SUM 🤝
#### promise 값의 

 
