# web3.version.node

返回节点软件信息。

同步调用：
```
web3.verison.node
```

异步调用：
```
web3.version.getNode(callback(error, result){ ... })
```

返回值：

- `String` - 客户端或节点的版本信息

示例：

```
//test.js 省略初始化过程
var version = web3.version.node;
console.log(version);
```

在终端执行脚本：
```
$ node test.js
EthereumJS TestRPC/v3.0.3/ethereum-js
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
