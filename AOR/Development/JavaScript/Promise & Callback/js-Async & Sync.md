#aor 
### Async
>[!note]
>#### 비동기 
>
>>Description

- 자바스크립트는 자바스크립트 엔진으로 단일 스레드로 모든 작업을 순차적으로 수행한다.
- 특정 연산에서 수행 시간이 오래 걸릴 경우 (ex. setTimeout(), HTTP request)
	- 해당 작업을 브라우저에서 Off-Load시켜 다중 스레드를 사용할 수 있게 한다.
	- Off-Load된 자바스크립트로 쓰여진 작업과 브라우저와 다시 소통해야 할 경우, 콜백 함수를 사용한다. 
	- Callback 함수를 사용시 브라우저의 다른 연산이 끝나면, 호출된다.
---
### Sync
>[!note]
>#### 동기 
>
>>Description

### [JavaScript](AOR/Dev-Index/JavaScript.md) Index로 돌아가기