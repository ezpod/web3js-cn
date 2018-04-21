# web3.net.peerCount

属性是只读的，返回连接节点已连上的其它以太坊节点的数量。

同步调用：
```
web3.net.peerCount
```

异步调用：
```
web3.net.getPeerCount(callback(error, result){ ... })
```

返回值：

- `Number` - 连接节点连上的其它以太坊节点的数量

示例：

```
var peerCount = web3.net.peerCount;
console.log("Peer count: " + peerCount); 
//Peer count: 0
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
