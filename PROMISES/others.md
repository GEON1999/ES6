.all, .race, .finally ✍️
=============
2nd header(opt) ☑
-------------

### .all 💬
#### 다수의 promise 컨트롤 가능 🔥
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
// output -> ['First', 'second', 'third']
```
+ 다수의 promise 의 값을 동시에 사용할 수도, 그중 오류가 있는 promise 가 있는지 검수할 수도 있음
+ 먼저 pending 이 끝난 promise 순서가 아닌, Promise.all(1, 2, 3) 안에 기재된 순서대로 값이 나열됨
 
 <br/>
 
 ### .race 💬
#### promise 중 가장 먼저 pending 이 완료된 값을 이행하거나 거부함 🔥
+ 예시
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

### .finally 💬
#### promise의 조건이 충족 여부와 관계 없이 promise 처리가 완료되면 무조건 실행되는 코드 🔥
+ 예시
 ```java
const p1 = new Promise((resolve, reject) => {
  setTimeout(reject, 1000, "First");
})
.then((value) => console.log(value))
.catch((e) => console.log(`${e}error`))
.finally(() => console.log("Im done"));
// output -> Firsterror / Im done
```
+ error 을 catch 하고 콘솔창에 출력했음에도 Im done 을 콘솔창에 출력함

 <hr/>
 
 
 ### SUM 🤝
#### promise의 다양한 메소드

 
