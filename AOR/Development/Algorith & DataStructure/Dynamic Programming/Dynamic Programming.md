- 반복되는 하위 문제 & 최적 부분 구조 


#aor 
### 동적 프로그래밍
>[!note]
>#### Dynamic Programing
>
>>복잡한 문제 -> 간단한 하위 문제의 모음
>>하위 문제들의 모음들의 답을 저장하는 방식으로 문제를 푸는 접근법

#### 언제 사용?
- 최적 부분 구조가 존재할 때 사용
    - 최적 부분 구조는 전체 도로를 지니고 있는 지도를 말한다.
    - 만일 고속도로만 지니는 지도라면 최적의 비용을 알 수 없다.
- 반복되는 하위 문제가 있을 때, 사용
	- 예시: 피보나치 수열(O) 병합정렬(X)
	- 인자가 반복되어 해결되는 하위 문제이다.

#### TOP-DOWN
memoization 
- 하위문제에 대한 결과 값을 저장할 수 있는 구조를 사용해 이전 결과에 대한 메모를 통해  시간복잡도를 단축시킨다.
- memoization은 재귀를 사용하기 때문에 공간복잡도가 tabulation보다 크다 (수가 클 경우 stackoverflow발생)
- 시간복잡도 O(N)

>[!note]
>>Richard Bellman - 동적 프로그래밍에서 동적이란 문제가 시간에 따라서 달라지는 양상을 묘사한다.

#### BOTTOM UP
tabulation
- 배열 테이블에 데이터를 저장하고 LOOP를 돌면서 상향식으로 덧셈을 하는 것
- 공간복잡도: tabulation < recursion(memoization)
- 시간복잡도: O(N)
### [JavaScript](../../../Dev-Index/JavaScript.md) Index로 돌아가기

