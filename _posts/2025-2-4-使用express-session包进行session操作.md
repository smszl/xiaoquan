**express-session对session进行操作**
安装express-session 与connect-mongo（进行session存储在mongo里面）
```javascript
npm i express-session connect-mongo
```
引入
```javascript
const session=require('express-session');
const mongostroe=require('connect-mongo');
```
设置中间件
```javascript
app.use(session({
name:"sid",   //设置cookie的名字 默认connect.sid
secret:"jiami",  //参与加密的字符串
saveUninitialized:false //是否为每次请求都设置一个cookie用来存储session发来的ids
resave:true    //是否在每次请求后保存session
store:MongoStore.create({
mongoUrl:'mongodb://127.0.0.27017/seesion'  //数据库的配置
}),
cookie:{
httpOnly:true,       //开启后前端无法通过js请求
maxAge:1000 * 30 //session过期时间
}
}));
```
