Arrow Function ✍️
=============

### What is Arrow function? 💬
#### 보기 편한 함수 🔥
+ arrow : =>
예제)
```java
//before
names.map(function(item) {return item + ","};
// arrow function
names.map(item => {return item + ","});
// implicit return : whatever i put in same line, it will be returned.
names.map(item => item + ",");
// argument 가 2개 이상인 경우 index 필요
names.map((item, index) => item + "," + index);
```

### This 💬
#### When we should now use arrow function 🔥
+ arrow function 안에 있는 this는 window 를 참조함   
- this 를 사용하고 싶다면 arrow function 을 사용해서는 안됨
 

 <hr/>
 
 
 ### SUM 🤝
#### 쓰기도, 보기도 쉬워진 함수
+ this 키워드 사용 시 arrow function 사용 x
+ 같은 줄에선 return 하지 않아도됨 ({} 사용 x)
+ 같은 줄이 아닌 경우엔 ({}) 과 같이 사용 시 return 생략 가능
 
