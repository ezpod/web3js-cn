# web3.toBigNumber

将给定的数字或十六进制字符串转为BigNumber。

调用：
```
web3.toBigNumber(value)
```

参数：

- `value`：	Number|String - 数字或十六进制格式的数字

返回值：

- `BigNumber` - BigNumber的实例

示例：
```
var value = web3.toBigNumber('200000000000000000000001');
console.log(value); // instanceOf BigNumber
console.log(value.toNumber()); // 2.0000000000000002e+23
console.log(value.toString(10)); // '200000000000000000000001'
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)


