**Node.js默认支持CommonJs规范，浏览器不支持所以需要编译。**
  
  1.全局安装browserify
```javascript
npm i -g browserify
```
2.编译自己要运行的nodejs文件
```javascript
browserify XXX.js -o ooo.js
xxx.js是源文件，ooo.js是输出的目标文件
```
3.页面中引用使用
```javascript
<script type="text/javascript" src="./ooo.js"></script>
```
