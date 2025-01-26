**安装依赖的步骤**
先执行npm init安装初始化package.json文件  
使用npm i -g nodemon 安装所需的依赖  
nodemon依赖安装完之后，可以在命令行的任意路径运行nodemon命令  
nodemon依赖包的作用 更新js文件后自动重启服务  
```javascript
nodemon ./xxx.js
```
可以通过npm root -g 查看全局安装包的位置  
只有全局类的工具适合全局安装,具体可以查看包的官方文档  
**错误**
当nodemon命令执行不了，就得去修改全局执行策略  
1.以管理员启动powershell命令行  
2.输入set-ExecutionPolicy remoteSigned  
3.选择A选项  
**小提示**
require()导入流程  
require()会去node_modules文件夹里面找package.json里面main属性中同名文件夹  
如果在相对js执行文件的路径里面没有node_modules文件，就会返回上一级目录寻找，直到找到本磁盘根目录
