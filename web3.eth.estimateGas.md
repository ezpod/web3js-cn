# web3.eth.estimateGas

估计调用需要耗费的gas量。这个方法在节点的VM中执行一个消息调用或交易，但是不会修改区块链。

调用：

```
web3.eth.estimateGas(callObject [, callback])
```

参数：

- `callObject`：	Object - 要发送的交易对象，可包含以下字段：
  - from: String - 指定的发送者的地址。如果不指定，使用web3.eth.defaultAccount。
  -	to: String - （可选）交易消息的目标地址，如果是合约创建，则不填.
  - value: Number|String|BigNumber - （可选）交易携带的货币量，以wei为单位。如果合约创建交易，则为初始的基金。
  - gas: Number|String|BigNumber - （可选）默认是自动，交易可使用的gas，未使用的gas会退回。
  - gasPrice: Number|String|BigNumber - （可选）默认是自动确定，交易的gas价格，默认是网络gas价格的平均值 。
  - data: String - （可选）或者包含相关数据的字节字符串，如果是合约创建，则是初始化要用到的代码。
  - nonce: Number - （可选）整数，使用此值，可以允许你覆盖你自己的相同nonce的，正在pending中的交易11。
- `callback`：Function - 回调函数，用于支持异步的执行方式


返回值：

- `Number` - 模拟的call/transcation花费的gas。

示例：
```
var result = web3.eth.estimateGas({
    to: "0xc4abd0339eb8d57087278718986382264244252f", 
    data: "0xc6888fa10000000000000000000000000000000000000000000000000000000000000003"
});
console.log(result); 
//输出 "0x0000000000000000000000000000000000000000000000000000000000000015"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
