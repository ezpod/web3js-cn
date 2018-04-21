# web3.toHex

将任何值转为HEX。

调用：

```
web3.toHex(val)
```

参数：

- `val`：String|Number|Object|Array|BigNumber - 需要转化为HEX的值。如果是一个对象或数组类型，将会先用JSON.stringify1进行转换成字符串。
  如果传入的是BigNumber2，则将得到对应的Number的HEX。

返回：

- `String`

示例：
```
//test.js - 初始化基本对象
var Web3 = require('web3');
var web3 = new Web3(new Web3.providers.HttpProvider("http://localhost:8545"));
var BigNumber = require('bignumber.js');

var str = "abcABC";
var obj = {abc: 'ABC'};
var bignumber = new BigNumber('12345678901234567890');

var hstr = web3.toHex(str);
var hobj = web3.toHex(obj);
var hbg = web3.toHex(bignumber);

console.log("Hex of Sring:" + hstr);
console.log("Hex of Object:" + hobj);
console.log("Hex of BigNumber:" + hbg);
```

在终端执行脚本：

```
$ node test.js
Hex of Sring:0x616263414243
Hex of Object:0x7b22616263223a22414243227d
Hex of BigNumber:0xab54a98ceb1f0ad2
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
