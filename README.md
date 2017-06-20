# jQuery-rating
jQuery rating (评分组件)


## 参数
```js
starkPic: 'images/stark2.png',	// 空的星星的图片
starPic: 'images/stars2.png',	// 填满星星的图片
starWidth: "32px",				// 图片的宽度
starHeigt: "21px",				// 图片的长度
clickFuc: function () {},		// 点击之后的回调函数
noclick: false,					// 是否可以点击，默认true, 如果设置为false, 需要设置下面的参数
index: 0,						// 显示到相应位置的信息，默认为0
text: '我是随意设置的文字',		// 默认显示的文字
```

## 例子
```
$('#div1').rating({
	"starkPic": 'images/starky.png',
	"starPic": 'images/starsy.png',
	"backgroundColor": '#000',
	"starWidth": "22px",
	"starHeigt": "21px",
	clickFuc: function (data) {
		alert('你点击了“' + data.text + '”, 它的值是：' + data.value );
	}
});

$('#div2').rating({
	starkPic: 'images/stark2.png',
	starPic: 'images/stars2.png',
	backgroundColor: '#000',
	starWidth: "32px",
	starHeigt: "21px",
	
	noclick: true,
	index: 3,
	text: '我是随意设置的文字',

	clickFuc: function (data) {
		alert('你点击了“' + data.text + '”, 它的值是：' + data.value );
	}
});
```

## 实例
- [demo](https://kuckboy1994.github.io/dailyNote/jQuery/component_jquery/rating/index.html)