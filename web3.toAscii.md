# web3.toAscii

将HEX字符串转为ASCII3字符串

调用：
```
web3.toAscii(hexString)
```

参数：

- `hexString`：String - 十六进制字符串。

返回值：

- `String` - 给定十六进制字符串对应的ASCII码值。

示例：
```
var str = web3.toAscii("0x657468657265756d000000000000000000000000000000000000000000000000");
console.log(str); // "ethereum"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
