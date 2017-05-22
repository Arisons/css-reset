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

###　animation
> animation属性是一个简写属性，用于设置六个动画属性：
> animation-name 规定需要绑定到选择器的keyframe名称
> animation-timing-function 规定完成动画所花费的时间，以秒或者毫秒计
> animation-delay 规定动画的速度曲线
> animation-iteration-count 规定动画应该播放的次数
> animation-direction 规定是否应该循环播放动画
** 注释： **请时钟规定animation-duration属性，否则时长为0，就不会播放动画了。

<table>
	<tr>
		<td>默认值</td>
		<td>none 0 ease 0 1 normal</td>
	</tr>
	<tr>
		<td>继承性</td>
		<td>no</td>
	</tr>
	<tr>
		<td>版本</td>
		<td>CSS3</td>
	</tr>
	<tr>
		<td>javascript语法</td>
		<td>object.style.animation="mymove 5s infinite"</td>
	</tr>
</table>

### transform

Internet Explorer10、Firefox、Opera支持transform属性

Internet Exploer 9 支持替代的-ms-transform属性（仅适用于2D转换）

Safari和Chrome支持替代的-webkit-transform属性（3D和2D转换）

Opera只支持2D转换

transform属性想元素应用2D或3D转换。该属性允许我们对元素进行旋转、缩放、移动或倾斜。

语法：transform: none | transform-functions;

<table>
	<tr>
		<td>值</td>
		<td>描述</td>
	</tr>
	<tr>
		<td>none</td>
		<td>定义不进行转换</td>
	</tr>
	<tr>
		<td>matrix(n,n,n,n,n,n)</td>
		<td>定义 2D 转换，使用六个值的矩阵</td>
	</tr>
	<tr>
		<td>matrix3d(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n)</td>
		<td>定义 3D 转换，使用 16 个值的 4x4 矩阵</td>
	</tr>
	<tr>
		<td>translate(x,y)</td>
		<td>定义 2D 转换</td>
	</tr>
	<tr>
		<td>translate3d(x,y,z)</td>
		<td>定义 3D 转换</td>
	</tr>
	<tr>
		<td>translateX(x)</td>
		<td>定义转换，只是用 X 轴的值</td>
	</tr>
	<tr>
		<td>translateY(y)</td>
		<td>定义转换，只是用 Y 轴的值</td>
	</tr>
	<tr>
		<td>translateZ(z)</td>
		<td>定义 3D 转换，只是用 Z 轴的值</td>
	</tr>
	<tr>
		<td>scale(x,y)</td>
		<td>定义 2D 缩放转换</td>
	</tr>
	<tr>
		<td>scale3d(x,y,z)</td>
		<td>定义 3D 缩放转换</td>
	</tr>
	<tr>
		<td>scaleX(x)</td>
		<td>通过设置 X 轴的值来定义缩放转换</td>
	</tr>
	<tr>
		<td>scaleY(y)</td>
		<td>通过设置 Y 轴的值来定义缩放转换</td>
	</tr>
	<tr>
		<td>scaleZ(z)</td>
		<td>通过设置 Z 轴的值来定义 3D 缩放转换</td>
	</tr>
	<tr>
		<td>rotate(angle)</td>
		<td>定义 2D 旋转，在参数中规定角度</td>
	</tr>
	<tr>
		<td>rotate3d(x,y,z,angle)</td>
		<td>定义 3D 旋转</td>
	</tr>
	<tr>
		<td>rotateX(angle)</td>
		<td>定义沿着 X 轴的 3D 旋转</td>
	</tr>
	<tr>
		<td>rotateY(angle)</td>
		<td>定义沿着 Y 轴的 3D 旋转</td>
	</tr>
	<tr>
		<td>rotateZ(angle)</td>
		<td>定义沿着 Z 轴的 3D 旋转</td>
	</tr>
	<tr>
		<td>skew(x-angle,y-angle)</td>
		<td>定义沿着 X 和 Y 轴的 2D 倾斜转换</td>
	</tr>
	<tr>
		<td>skewX(angle)</td>
		<td>定义沿着 X 轴的 2D 倾斜转换</td>
	</tr>
	<tr>
		<td>skewY(angle)</td>
		<td>定义沿着 Y 轴的 2D 倾斜转换</td>
	</tr>
	<tr>
		<td>perspective(n)</td>
		<td>为 3D 转换元素定义透视视图</td>
	</tr>
</table>
*	rotate
*	translateY
