```javascript
<ul>
    <li v-for="i in games" :key="i.id">{{ i.name }}</li>
 </ul>
```
代码在Vue3运行  
v-for 指令遍历了 games 数组，并在每次迭代时将当前项赋值给 i，然后在模板中进行渲染。每个li列表都有一个唯一的 key 属性,为了方便就把games数组里面的id赋给了key。  
：等价于v-bind就是为了使key的""字符串变成值，让值可以动态更新
