# web3.net.listening

此属性是只读的，表示当前连接的节点，是否正在监听网络连接。

同步调用：
```
web3.net.listening
```

异步调用：
```
web3.net.getListener(callback(error, result){ ... })
```

返回值：

- `Boolean` - true表示连接上的节点正在监听网络请求。

示例：
```
var listening = web3.net.listening;
console.log("client listening: " + listening);
//client listening: true
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
