**配置package.json文件中的script属性**  
```javascript
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
	"start":"node index.js"
  }
```
配置完之后，可以使用配置的别名进行命令操作  
```javascript
npm run start
```
**注意：**start比较特殊，可以省略run
```javascript
npm start
```
**补充说明**  
```javascript
npm start一般用于启动项目
```
*npm run*跟*require()*函数一样，寻找指定路径的文件，如果在当前目录没有找到就会返回上一级继续寻找，直到找到或者找到磁盘根目录还没有目标文件，就报错。
