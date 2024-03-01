#aor 
### type
>[!note]
>#### 타입
>
>>핵심 타입: `number` `boolean` `string`

### number
```ts
function num(n1: number) {
	console.log(n1);
};
const number1 = 3;
num(number1); // 3
```
### boolean
```ts
function bool(n1: boolean) {
	console.log(n1);
};
const number1 = true;
num(number1); // true
```
### string
```ts
function str(n1: string) {
	console.log(n1);
};
const number1 = 'hi';
num(number1); // hi
```
### object
- 잘못된 예시
```ts
// <- 아래 예시의 경우 타입스크립트는 `person`을 아무런 정보가 없는 객체라고 파악해 오류를 일으킨다.
const person: object = { 
	name: 'yoon',
}
console.log(person.name); // error
```
- 올바른 예시
```ts
// 위와 같이 객체에 대한 구체적인 정보를 기입해야 컴파일러에서 오류가 나지 않는다.
const person: {
	name: string,
	age: number
} = { 
	name: 'yoon',
	age: 28,
}
console.log(person.name); // 'yoon'
```
- 중첩 객체의 경우 (응용)
```ts
const product: {
  id: string;
  price: number;
  tags: string[];
  details: {
    title: string;
    description: string;
  }
} = {
  id: 'abc1',
  price: 12.99,
  tags: ['mz세대', '타입스크립트'],
  details: {
    title: '프론트엔드 직무를 위한 책',
    description: 'a great book for the Front-end Dev'
  }
}
```
### 배열
- `string[]`
```ts
const array: string[] = ['hi', 'my name is ', 'yoon'];
```
- `any[]`
```ts
const array: any[] = [6, 'hi', true];
```
### 튜플
```ts
// 두가지 이상의 타입을 사용하기 위한 배열
const array: [number, string] = [6, 'hi'];
array.push('hello'); // <-- 튜플에서 허용되는 예외, 타입스크립트 컴파일러가 오류를 직접 잡을 수 없다.
```
### [TypeScript](../../Dev-Index/TypeScript.md) Index로 돌아가기