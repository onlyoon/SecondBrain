#aor 
### webkit
>[!note]
>#### 웹킷
>
>>Chrome과 Safari 등의 브라우저에 탑재된 엔진으로서, 해당 브라우저에만 작동하는 웹 브라우저 렌더링 엔진([[css-web rendering engine]])
>
>>애플이 오픈소스로 개발하고 있는 웹 브라우저 렌더링 엔진

- webkit 동작 과정
![[Pasted image 20230930174238.png]]

### Web Browser Engine
>[!note]
>#### 웹 브라우저 엔진
>
>>UI와 렌더링 엔진을 연결하는 엔진

### Web Rendering Engine
>[!note]
>#### 웹 렌더링 엔진
>
>>요청받은 내용을 브라우저 화면에 표시하는 일을 한다.
>
>>HTML과 CSS를 주로 사용

- 동작과정
	1. HTML 파일 파싱
	2. 파싱된 태그 DOM 노드로 전환
	3. CSS 파일 파싱
	4. 파싱된 HTML & CSS 파일을 가지고 렌더 트리 생성
	5. 렌더 트리를 기반으로 배치 및 그리기
	6. 완료된 화면 표시



### [CSS](../../Dev-Index/CSS.md) Index로 돌아가기