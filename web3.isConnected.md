# web3.isConnected
检查是否与节点连接上。

调用：
```
web3.isConnected()
```

参数：
- 无

返回值：

- `Boolean`：true表示已连接

示例：
```
//省略初始化过程
var connected = web3.isConnected();
if(!connected){
  console.log("node not connected!");
}else{
  console.log("node connected");
}
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
