#aor 
- 출처
	- https://developer.mozilla.org/ko/docs/Web/API/XMLHttpRequest
### XMLHttpRequest
>[!note]
>#### XMLHttpRequest 객체
>
>>서버와 프로토콜로 상호작용하기 위해서 사용하는 통신 객체
#### 코드 예시
```js
const xhr = new XMLHttpRequest();

// XMLHttpRequest를 초기화하는 메서드
xhr.open('GET', 'https://jsonplaceholder.typicode.com/posts');

// JSON 객체로 받은 응답을 구문분석해주는 메서드
xhr.responseType = 'json';

// 요청을 보낸 이후의 load event를 기다리기 위한 event listener 생성 메서드
xhr.onload = function() {
	...
}

// XMLHttpRequest를 서버에 전달하는 메서드
xhr.send();

```
#### load event
- 데이터가 로딩된 이후(요청이 완료되면) 자동으로 실행되는 이벤트이다.
### [JavaScript](AOR/Dev-Index/JavaScript.md) Index로 돌아가기