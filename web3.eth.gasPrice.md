# web3.eth.gasPrice

返回当前的gas价格。这个值由最近几个块的gas价格的中值决定。只读属性。

同步调用：

```
web3.eth.gasPrice
```
异步调用：

```
web3.eth.getGasPrice(callback(error, result){ ... })
```

返回值：

- `BigNumber` - 当前的gas价格的BigNumber实例，以wei为单位。

示例：
```
var gasPrice = web3.eth.gasPrice;
console.log(gasPrice.toString(10)); // "10000000000000"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
