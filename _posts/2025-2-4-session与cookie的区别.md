**session与cookie的区别**
1.存在的位置
```html
cookie:浏览器端
session:服务器端
```
2.安全性
```html
cookie以明文方式存放在浏览器端，安全性较低
session存放在服务器中，相对安全
```
3.网络传输量
```html
cookie设置内容过多会导致报文体积大，引起传输速度慢
session数据存放在服务器，只用cookie传输id,不会影响速率
```
4.存储限制
```html
浏览器限制单个cookie保存数据不能超过4k，并对单个域名的传输数量也有限制
session没有限制
```
