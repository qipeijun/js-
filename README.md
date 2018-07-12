
### 参照 @Ben.Luo 童鞋的项目，对方法进行改造，增加倒计时结束后的事件回调和 及时清除定时器;

# Countdown
js倒计时插件，无需依赖jquery，zepto等，适合简易页面，节省资源，**支持模块化**
### 使用方法
```js
new Countdown(el, options);
```
### 参数
```js
{
 format: "hh小时mm分ss秒" | "hh:mm:ss", 
 lastTime: "2016-04-20 16:00:00" | 1492675200000,
 callback: function () {
			console.log('我的倒计时结束啦');
	}
}
```
### 例子
```html
<h3 id="countdown1"></h3>
```
```js
new Countdown(document.getElementById('countdown1'),{
   format: "hh小时mm分ss秒",
   lastTime: "2017-04-20 16:00:00",
   callback: function () {
			console.log('我的倒计时结束啦');
		}
});
```
format:可以自定义输出格式  
lastTime: 倒计时截止的时间
callback:倒计时结束回调

### License
[MIT](https://opensource.org/licenses/MIT)