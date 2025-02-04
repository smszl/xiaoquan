**express框架里面获取cookie
下载cookie-parser安装包**
```javascript
npm i cookie-parser
```
导入cookie-parser包
```javascript
const cookieparser=require('cookie-paeser');
//全局路由
app.use(cookieparser());
```
获取cookie
```javascript
app.get('get-cookie',(request,response){
//获取cookie
console.log(response.cookies);
response.send('获取成功);
});
```
