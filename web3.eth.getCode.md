# web3.eth.getCode

获取链上指定地址的代码

调用：

```
web3.eth.getCode(addressHexString [, defaultBlock] [, callback])
```

参数：

- `addressHexString`：	String - 要获得代码的地址。
- `defaultBlock`：	Number|String -（可选）如果未传递参数，默认使用web3.eth.defaultBlock定义的块，否则使用指定区块。
- `callback`：	Function - 回调函数，用于支持异步的方式执行。

返回值：

- `String` - 给定地址合约编译后的字节代码。

示例：
```
var code = web3.eth.getCode("0xd5677cf67b5aa051bb40496e68ad359eb97cfbf8");
console.log(code); 
//"0x600160008035811a818181146012578301005b601b6001356025565b8060005260206000f25b600060078202905091905056"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
