# web3.reset

用来重置web3的状态。重置除了manager以外的其它所有东西。卸载filter，停止状态轮询。

调用：

```
web3.reset(flag)
```

参数：

- `flag`：Boolean - 如果设置为true，将会卸载所有的filter，但会保留web3.eth.isSyncing()的状态轮询。

返回值：

- 无

示例：
```
//test.js - 省略初始化过程
console.log("reseting ... ");
web3.reset();
console.log("is connected:" + web3.isConnected());
```

终端运行脚本：
```
$ node test.js
reseting ...
is connected:true
```
教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
