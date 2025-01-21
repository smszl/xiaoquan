```javascript
const fs=require('fs');
//准备写入的数据追加
const txt='一只小鸡地上走,两只青蛙刚刚骄。'
fs.appendFile('./文本.txt',txt,(err)=>{
    if(err==null){
        console.log('追加成功');
    }
});
//fs.appendFileSync：是一个同步方法，会阻塞其他代码执行，直到操作完成。如果发生错误，会抛出异常。
//fs.appendFile：是一个异步方法，不会阻塞下面其他代码执行，而是使用回调函数来处理错误和完成。
fs.appendFileSync('./文本.txt','lalala');
```
