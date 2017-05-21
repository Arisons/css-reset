## 1.沿着路径的动画

js代码：

```js

@keyframes spin {
	from {
		transform: rotate(0turn) translateY(-150px) translateY(50%) rotate(1turn)
	}
	to {
		transform: rotate(1turn) translateY(-150px) translateY(50%) rotate(0turn);
	}
}
.avatar {
	animation spin 3s infinite linear;
}

```

要研究的属性：

*	animation
*	transform
*	rotate
*	translateY
