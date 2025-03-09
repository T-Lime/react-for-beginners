# 노마드코더 ReactJS 입문
## ReactJS로 영화 웹 서비스 만들기
### 학습 내용을 저장해놓은 공간입니다.
* 같은 결과물의 JS와 ReactJS를 만들고 비교해보기.

----
### ReactJS를 사용하는 이유
* 자바스크립트를 보다 간편하게 만들 수 있음.
    * JS에서 HTML에 접근해서 간단한 작업을 할 때 보다 더 많은 시간이 소모됨

----
#### React JS
* 어플리케이션이 interactive하도록 만들어주는 라이브러리, 엔진
* React JS에서는 모든 것이 JS로써 시작.
* 유저에게 보여질 내용을 컨트롤 할 수 있음.
* element 업데이트를 HTMl에 보여주는 역할을 함
* property에다가 event listener를 등록할 수 있다.
    * on + event는 event listener인 것을 알고 있다.
----
### React-dom(library or package)
* react-dom : 모든 React element들을 HTML body에 두는 역할을 함.
* ReactDOM.render(생성한 태그(변수), 부모 태그(변수)) : React element를 가지고 HTML로 만들어 배치한다
    * 사용자에게 보여준다는 의미

----
* 변수명은 태그와 같지 않아도 된다.
* 속성에는 event listener를 등록할 수 있다. (onClick을 넣고 바로 함수를 넣을 수 있음)
    * HTML 문서에서 리액트 없이 바로 속성으로 onClick을 넣고 함수를 추가해서 사용할 수 있음.
    * JS에서는 click, HTML 속성에서는 onClick
```
// ("태그명", {속성}, 콘텐츠 내용)

const btn = React.createElement("button", {
            onClick: ()=> console.log('im clicked'),
        }, "Click me");
```
----
### 알아둬야 할 것!
* style={{backgroundColor:"tomato"}}
    * style은 {}가 2개이다.
* React에서 대문자로 시작하는 변수는 컴포넌트로 인식됨
    * 직접 만든 요소는 전부 대문자로 시작해야함
    * 함수로 정의를 해줘야함
* </태그명> 태그명이 소문자이거나 /가 태그명 앞에 있으면 HTML 태그로 인식하고
    * <변수명/> 리액트로 생성한 컴포넌트다 앞글자는 대문자로 해야 인식을 한다.