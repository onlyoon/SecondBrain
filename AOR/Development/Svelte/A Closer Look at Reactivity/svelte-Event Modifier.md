#aor
### Event Modifier
>[!note]
>이벤트 수식어
>
>이벤트 구문 뒤에 추가하는 수식어(Modifier)

>[!example]
>>`on:Click|once`
>>`on:Click|passive`
>>`on:Click|capture`
>>`on:Click|stopPropagation` ([[js-event.stopPropagation()]])
>>`on:Click|preventDefault` ([[js-event.preventDefault()]])

사용법 :
```html
<script>
let count = 0;
function add() {
	count += 1;
}
</script>

<button on:click|preventDefault={add}>{count}</button>
```

사용하지 않았을 경우 :
```html
<script>
let count = 0;
function add(event) {
	event.preventDefault();
	count += 1;
}
</script>

<button on:click={add}>{count}</button>
```

### [Svelte](../../../Dev-Index/Svelte.md) index로 돌아가기