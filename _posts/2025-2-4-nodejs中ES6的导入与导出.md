**ES6的导出与导入**
  
  1.导出xxx.js里面其中一个变量
```javascript
export const name='张三';
```
2.导入xxx.js文件
```javascript
import * as name from './xxx.js';
console.log(name);
```
3.存在package.json文件
```json
{
	"type":"module"
}
```
