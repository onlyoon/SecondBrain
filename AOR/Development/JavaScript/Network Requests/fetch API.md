#aor 
### fetch API
>[!note]
>#### fetch API
>
>>서버와 프로토콜로 상호작용하기 위해, 사용하는 API
>
>>[XMLHttpRequest](AOR/Development/JavaScript/Network%20Requests/XMLHttpRequest.md)를 보완한 자바스크립트의 최신형 API, 구세대 브라우저에서 지원하지 않는다.
>
>>[Promise](AOR/Development/JavaScript/Promise%20&%20Callback/Promise.md)를 기반으로 한 함수이자, 함수 자체적으로 지원해 [Promise](AOR/Development/JavaScript/Promise%20&%20Callback/Promise.md) 객체를 반환하는 API이다.
>
>>fetch API는 파싱된 응답이 아닌, 스트리밍된 응답을 반환한다.
#### 코드 예시
- fetch API는 `xhr.response`가 주는 파싱된 응답이 아닌, 스트리밍된 응답을 반환한다.
	- 이 응답을 가지고 `response` 객체에 대해 `json()`메서드를 호출하면, fetch API가 response 본문을 스냅샷을 찍은 후, 파싱해 JSON객체를 자바스크립트 코드로 변환하는 작업을 한다.
- fetch API의 두번째 인자에 `method`, `body` 프로퍼티가 들어가야 하며, 추가적으로 `header` 프로퍼티를 넣을 수 있다.
```js
const sendHttpRequest = (url, method, data) => {
    return fetch(url, {
	    method: method,
	    body: JSON.stringify(data),
	    header: {
		    'Content-Type': 'application/json'
	    }
    }).then(response => {
        return response.json();
    });
};
```

>[!warning]
>>fetch API의 추가 메서드를 통해 JSON객체의 데이터 뿐만 아니라, 스냅샷으로 반환해야 하는, 스트리밍 데이터를 얻을 수 있다.
### [JavaScript](../../../Dev-Index/JavaScript.md) Index로 돌아가기