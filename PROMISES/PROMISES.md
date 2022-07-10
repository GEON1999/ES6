 PROMISES ✍️
=============
Promise 객체는 비동기 작업이 맞이할 미래의 완료 또는 실패와 그 결과 값을 나타냅니다. ☑
-------------

### What is Promise 💬
#### 요약 🔥
Promise는 프로미스가 생성된 시점에는 알려지지 않았을 수도 있는 값을 위한 대리자로, 비동기 연산이 종료된 이후에 결과 값과 실패 사유를 처리하기 위한 처리기를 연결할 수 있습니다.
프로미스를 사용하면 비동기 메서드에서 마치 동기 메서드처럼 값을 반환할 수 있습니다. 다만 최종 결과를 반환하는 것이 아니고,
__미래의 어떤 시점에 결과를 제공하겠다는 '약속'(프로미스)을 반환합니다.__   
   
    
+ 대기(pending): 이행하지도, 거부하지도 않은 초기 상태.
+ 이행(fulfilled): 연산이 성공적으로 완료됨.
+ 거부(rejected): 연산이 실패함.


 ```java
 const amIsmart = new Promise((resolve, resject) => {
  setTimeout(resolve, 3000, "maybe");
})
 
 amIsmart.then(string => console.log(string))
 
 console.log("hi")
// output -> hi / maybe
```
+ 소스코드가 순서대로 실행된다면 maybe 가 출력되고 이후 hi 가 출력되어야 한다. 그러나 promise 가 이행되었을 때 then 을 호출하기에 hi 가 우선 출력됨

 <hr/>
 
 ### SUM 🤝
#### 약속
 
 
