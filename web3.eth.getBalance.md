# web3.eth.getBalance

返回链上指定地址的账户余额。

调用：
```
web3.eth.getBalance(addressHexString [, defaultBlock] [, callback])
```
参数：

- `addressHexString`：	String - 要查询余额的地址。
- `defaultBlock`：	Number|String -（可选）如果不设置此值，将使用`web3.eth.defaultBlock`设定的块，否则使用指定的块。
- `callback`：	Funciton - （可选）回调函数，用于支持异步的执行方式。
返回值：

- `String` - 一个包含给定地址的当前余额的BigNumber实例，单位为wei。

示例：
```
var balance = web3.eth.getBalance("0x407d73d8a49eeb85d32cf465507dd71d507100c1");
console.log(balance); // instanceof BigNumber
console.log(balance.toString(10)); // '1000000000000'
console.log(balance.toNumber()); // 1000000000000
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
