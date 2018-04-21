# web3.version.whisper

返回whisper协议版本。

同步调用：
```
web3.version.whisper
```

异步调用：
```
web3.version.getWhisper(callback(error, result){ ... })
```

返回值：

- `String` - whisper协议的版本

示例：
```
//省略初始化过程
var version = web3.version.whisper;
console.log(version);
//20
```

注意：EthereumJS testRPC客户端不支持这个命令，报错Error: Error: RPC method shh_version not supported.

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
