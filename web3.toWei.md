# web3.toWei

将给定资金转换为以wei为单位的数值。

调用：
```
web3.toWei(number, unit)
```
参数：

- `number`：Number|String|BigNumber - 数字或BigNumber
- `unit` ： String - 字符串单位

可选择的单位如下：

- kwei/ada
- mwei/babbage
- gwei/shannon
- szabo
- finney
- ether
- kether/grand/einstein
- mether
- gether
- tether

返回值：

- `String|BigNumber` - 根据传入参数的不同，分别是字符串形式的字符串，或者是BigNumber。

示例：
```
var value = web3.toWei('1', 'ether');
console.log(value); // "1000000000000000000"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
