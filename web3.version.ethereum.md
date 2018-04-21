# web3.version.ethereum

返回以太坊的协议版本。

同步调用：
```
web3.version.ethereum
```

异步调用：
```
web3.version.getEthereum(callback(error, result){ ... })
```

返回值：

- `String` - 以太坊的协议版本

示例：
```
//省略初始化过程
var version = web3.version.ethereum;
console.log(version);
// 60
```

注意：EthereumJS testRPC客户端不支持这个命令，报错Error: Error: RPC method eth_protocolVersion not supported.
