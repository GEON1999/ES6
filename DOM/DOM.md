# DOM
- 브라우저의 렌더링 엔진은 HTML 문서를 파싱하여 브라우저가 이해할 수 있는 자료구조인 DOM을 생성한다.
- DOM(Document Object Model)은 HTML 문서의 계층적 구조와 정보를 표현하며 이를 제어할 수 있는 API, 즉 프로퍼티와 메소드를 제공하는 트리 자료구조다.

</br></br>

## 노드

</br>

### 1. HTML 요소와 노드 객체
- HTML 요소는 렌더링 엔진에 의해 파싱되어 DOM을 구성하는 요소노드 객체로 변환된다.
- 이때 요소노드 내 어트리뷰트는 어트리뷰트 노드로, 텍스트 콘텐츠는 텍스트 노드로 변환된다.
<div>
<img height="500" src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FeneUyh%2FbtqYhykABfP%2F4iXHfbp2FgkaHIh2yJ6nKk%2Fimg.png"/>
</div>

- HTMl 문서는 요소들의 집합으로 이루어지며, HTML 요소는 중첩 관계를 갖는다.
- 중첩된 관계에서 계층적인 부자 관계가 형성된다. 
- 이러한 HTML 요소간 부자 관계를 반영하여 HTML 요소를 객체화한 모든 노드 객체들을 __트리 자료구조__ 로 구성한다.
  - 트리구조 내 최상위 노드는 부모가 없으며, __루트 노드__ 라 하고, 자식 노드가 없는 노드를 __리프 노드__ 라 한다.
- 노드 객체들로 구성된 트리 자료구조를 DOM 이라고 한다. (노드 객체의 트리로 구조화 되어있어, DOM을 DOM트리 라고도 한다.
