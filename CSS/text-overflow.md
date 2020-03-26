### 文本溢出解决方案
#### 核心属性设置
1. `overflow: hidden;`：内容长度超出指定宽度，则隐藏超出的内容
2. `white-space: nowrap;`：设置文字在一行显示，不换行
3. `text-overflow: ellipsis;`：当文本溢出时，以省略号代替显示被截掉的文本
#### 单行文本溢出
```
p {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
```

#### 多行文本溢出
```
p {
  display: -webkit-box; // 将对象作为弹性盒子伸缩展示
  -webkit-line-clamp: 2; // 文本行数
  -webkit-box-orient: vertical; // 设置子元素排列方式
  overflow: hidden;
  text-overflow: ellipsis;
}
```