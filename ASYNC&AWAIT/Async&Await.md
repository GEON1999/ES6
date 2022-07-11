Async&Await ✍️
=============
코드의 구문과 구조가 표준 동기 함수와 비슷한 비동기 함수 ☑
-------------

### Why Async&Await and how to use it? 💬
#### 암시적으로 Promise를 사용하여 결과를 반환하지만 동기 함수와 비슷한 구조로서 쓰고 읽기에 용이함 🔥
+ 예시
 ```java
const getNowPlayingMovies = async() => {
  try{
    const response = await fetch('https://api.themoviedb.org/3/movie/now_playing?api_key=<<api_key>>');
    const json = await responese.json();
    console.log(json);
    } catch(error) {
      console.log(error)
    } finally {
      console.log("it's finished")
    }
}

getNowPlayingMovies()
// api key 는 보안의 문제로 기재하지 않음
```

 <hr/>
 
 
 ### SUM 🤝
#### Promise()'s Upgrade version
+ 간결하여 쓰고 읽기 편하며 error 핸들링 또한 편함
 
