**RESTful API是一种特殊风格的接口，主要特点有如下几个:**  
1.URL路径中不能有动词  
2.操作方法要与HTTP请求方法对应  
3.操作结果要与HTTP响应状态码对应

**json-server工具**
作用：可以快捷搭建RESTfulAPI服务  
全局安装json-server
```javascript
npm i -g json-server
```
创建json文件，编写基本结构
```json
{
    "song":[
        {
            "id":1,
            "name":"关山酒",
            "singer":"三月红"
        },
        {
            "id":2,
            "name":"不能说的秘密",
            "singer":"小尼姑"
        }
    ]
}
```
以json文件(XXX.json)所在文件为工作目录，执行下面命令
```javascript
json-server --watch XXX.json  //默认listen端口为3000
```
详情官网github.com/typicode/json-server
