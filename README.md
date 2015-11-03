# css-hack2
<h4><a href="http://css.doyoe.com/">属性级Hack</a></h4>

<pre>
取值：
_：
选择IE6及以下。连接线（中划线）（-）亦可使用，为了避免与某些带中划线的属性混淆，所以使用下划线（_）更为合适。
*：
选择IE7及以下。诸如：（+）与（#）之类的均可使用，不过业界对（*）的认知度更高
\9：
选择IE6+
\0：
选择IE8+和Opera15以下的浏览器


如想同一段文字在IE6,7,8显示为不同颜色，可这样写：
.test {
	color: #090\9; /* For IE8+ */
	*color: #f00;  /* For IE7 and earlier */
	_color: #ff0;  /* For IE6 and earlier */
}
* 上述Hack均需运行在标准模式下，若在怪异模式下运行，这些Hack将会被不同版本的IE相互识别，导致失效。

</pre>
