#aor 
### Promise
>[!note]
>#### 프로미스 객체
>
>>여러 개의 중첩된 콜백 지옥 대신 사용하는 객체이며, 하나의 중첩 레벨을 사용해 코드를 가독성있게 만들어 준다.

#### resolve 함수
- Promise 객체의 [Callback Function](AOR/Development/JavaScript/Advanced%20Function/Callback%20Function.md)(executor)에서 사용되는 함수로서 해당 함수가 호출되면, Promise객체가 내부적으로 해결됨(SUCCESS)을 표시하는 함수
- 해결됨을 알리기 위한 인자를 넣는 것이 가능하다.
#### reject 함수
- Promise 객체의 [Callback Function](AOR/Development/JavaScript/Advanced%20Function/Callback%20Function.md)(executor)에서 사용되는 함수로서 해당 함수가 호출되면, Promise객체가 내부적으로 실패함(FAIL)을 표시하는 함수
- 실패함을 알리기 위한 인자를 넣는 것이 가능하다.

- 예시
```js
const setTimer = (duration) => {
	// 프로미스 객체 생성
	// 함수 인자(executor)는 프로미스 객체가 생성될 때 즉각 호출된다.
	const promise = new Promise((resolve, reject) => {
		setTimeout(() => {
			resolve();
		}, duration);
	});
	return promise;
};

setTimer(2000).then(data => {
	console.log(data, posData);
}); // <- setTimer() 함수는 Promise 객체를 반환하며, `then`키워드를 통해, Promise객체의 데이터를 가지고 다음 콜백 함수로 넘어갈 수 있다.
```

### [JavaScript](AOR/Dev-Index/JavaScript.md) Index로 돌아가기