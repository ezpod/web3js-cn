# web3.fromAscii

将任何的ASCII码字符串转为HEX字符串。

调用：
```
web3.fromAscii(textString,[padding])
```

参数：

- `textString`：String - ASCII码字符串
- `padding`：	Number - 返回的字符串字节大小，不够长会自动填充。

返回值：

- `String` - 转换后的HEX字符串。

示例：
```
//test.js
var str = web3.fromAscii('ethereum');
console.log(str); // "0x657468657265756d"

var str2 = web3.fromAscii('ethereum', 32);
console.log(str2); // "0x657468657265756d000000000000000000000000000000000000000000000000"
```

在终端执行脚本：
```
$ node test.js
0x657468657265756d
0x657468657265756d
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)

