```javascript
const http = require("http"); const server = http.createServer((request,response)=>{ response.end("来自 nidejs 服务器的问候"); });

const 端口=8181; const ip="127.0.0.2";

server.listen(port,ip,()=>{ console.log("服务运行在http://"+ip+":"+port); }); 
```
### 创建一个HTTP实例服务器，并通过listen()方法将服务器绑定到本机IP和端口8181上;
### 本机回环地址的范围是127.0.0.0/8，即从127.0.0.0到127.255.255.255‌。其中， 127.0.0.1是最常用的本地回环地址，也被称为localhost，它可以用来测试软件与本机的进程通信。
