# web3.version.network

返回所连接以太坊网络的network_id。

同步调用：
```
web3.version.network
```

异步调用：
```
web3.version.getNetwork(callback(error, result){ ... })
```

返回值:

- `String` - 网络协议版本

示例：

```
//省略初始化过程
var network = web3.version.network;
console.log(network);
//1488546587563
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
