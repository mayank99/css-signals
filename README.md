# css-signals

CSS custom properties + JS events as a state management solution?

```js
const [count, setCount] = createStore('--count');

document.body.addEventListener('--count', () => {
	console.log(count());
});

button.onclick = () => setCount(+count() + 1);
```
