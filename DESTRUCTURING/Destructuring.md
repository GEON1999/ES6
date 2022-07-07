Destructuring ✍️
=============
Object, Araay 등의 요소들 안 변수를 외부에서 사용할 수 있도록 하는 것 ☑
-------------

### Object Destructuring? 💬
#### Shortcut 🔥
 ```java
const settings = {
  notifications: {
    follow: true,
    alerts: true,
    unfolow: false,
   },
  color: {
    theme: "dark",
  },
};

const {
  notifications: { follow },
  color,
 } = settings;
 // 위 코드는 const follow = settings.notifications. follow, const color = settings.color 과 같은 효과를 함
```
+ 위와 같은 방식으로 코딩을 하면, settings 오브젝트 내에 있는데 요소들을 외부에 선언하고 사용하기 용이함
+ 반복되는 코딩을 줄이고 실수를 줄일 수 있음
 ```java
 const {
  notifications: { follow = false } = {} ,
  color,
 } = settings;
```
+ 위와 같이 default value 를 설정해줄 수도 있음 (notifications 가 없을 때 {} 빈 오브젝트를 그안엔 follow = false 값을 가짐)
 ```java
 const {
  notifications:{ follow: followMe = false },
  color,
 } = settings;
```
+ 위 코드와 같이 follow 의 이름을 변경할 수 있음

### Object Destructuring in function 💬
#### Shortcut 🔥
 ```java
function saveSettings(settings) {
  console.log(settings.followAlert);
  console.log(settings.unfollowAlert);
}

saveSettings({
  followAlert: true,
  unfollowAlert: true,
  mrkAlert: true,
  themeColor: "green",
});
```
+ 위 코드에서 followAlert 및 unfollowAlert 등의 값을 saveSettings 함수 안에서 사용하려면 settings property 내부의 요소에 접근 해야함
#### Shortcut 🔥
 ```java
function saveSettings({followAlert, unfollowAlert}) {
  console.log(followAlert);
  console.log(unfollowAlert);
}
```
+ Destructuring 을 사용하면 saveSettings 오브젝트 내부에 요소 자체를 property로 선언 및 사용 가능함

### Value Shorthands 💬
#### Shortcut 🔥
 ```java
const follow = checkFollow();
const alert = checkAlert();

const settings = {
  notifications: {
    follow,
    alert,
  },
};
```
+ follow : follow , alert : alert 를 짧게 코딩 가능함


### Others (array) 💬
#### Shortcut 🔥
 ```java
const days = ["mon", "tue", "wed", "thu", "fri"];
const [mon,tue] = days;
console.log(mon, tue);
// output -> "mon", "tue"

// 값을 skip 하고 싶으면 아래와 같이 사용 가능
const [, , , thu, fri] = days;
console.log(thu, fri);
// output -> "thu", "fri"
```
 <hr/>
 
 
 ### SUM 🤝
#### 특정 object 내 다수의 요소들을 사용할 경우, 극강의 효율을 발휘할 수 있는 Destructuring
