# web3.eth.accounts

只读属性，返回当前节点持有的帐户列表。

同步调用：
```
web3.eth.accounts
```
异步调用：
```
web3.eth.getAccounts(callback(error, result){ ... })
```

返回值：

- `Array` - 节点持有的帐户列表。

示例：
```
var accounts = web3.eth.accounts;
console.log(accounts); 
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
