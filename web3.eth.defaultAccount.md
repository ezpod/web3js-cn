# web3.eth.defaultAccount

设置在使用下述方法时使用的默认账户地址：

- web3.eth.sendTransaction()
- web3.eth.call()

你也可以选择通过指定from属性，来覆盖这个默认设置。

调用：
```
web3.eth.defaultAccount
```

返回值：

- `String` - 20字节的当前设置的默认地址。

示例：
```
//test.js
console.log("Current default: " + web3.eth.defaultAccount);
web3.eth.defaultAccount = '0x8888f1f195afa192cfee860698584c030f4c9db1';
console.log("Current default: " + web3.eth.defaultAccount);
```

在终端执行脚本：
```
$ node test.js
Current default: undefined
Current default: 0x8888f1f195afa192cfee860698584c030f4c9db1
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
