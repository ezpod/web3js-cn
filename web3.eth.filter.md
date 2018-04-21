# web3.eth.filter

监听合约事件。

调用：
```
web3.eth.filter(array (, options) )
```

参数：

- 	`array`：String|Object - 字符串的可取值[latest，pending]。latest表示监听最新的区块变化，pending表示监听正在pending的区块。如果需要按条件对象过滤，如下：
  - fromBlock: Number|string - 起始区块号（如果使用字符串latest，意思是最新的，正在打包的区块），默认值是latest。
  - toBlock: Number|string - 终止区块号（如果使用字符串latest，意思是最新的，正在打包的区块），默认值是latest。
  - address: String - 单个或多个地址。获取指定帐户的日志。
  - topics: String[] - 在日志对象中必须出现的字符串数组。顺序非常重要，如果你想忽略主题，使用null。如，[null,'0x00...']，你还可以为每个主题传递一个单独的可选项数组，如[null,['option1','option1']]。

返回值：

`Object` - 有下述方法的过滤对象：

-	filter.get(callback): 返回满足过滤条件的日志。
-	filter.watch(callback): 监听满足条件的状态变化，满足条件时调用回调。
-	filter.stopWatching(): 停止监听，清除节点中的过滤。你应该总是在监听完成后，执行这个操作。

监听回调的返回值：

-	String - 当使用latest参数时。返回最新的一个区块哈希值。
-	String - 当使用pending参数时。返回最新的pending中的交易哈希值。
-	Object - 当使用手工过滤选项时，将返回下述的日志对象。
  -	logIndex: Number - 日志在区块中的序号。如果是pending的日志，则为null。
  - transactionIndex: Number - 产生日志的交易在区块中的序号。如果是pending的日志，则为null。
  -	transactionHash: String，32字节 - 产生日志的交易哈希值。
  - blockHash: String，32字节 - 日志所在块的哈希。如果是pending的日志，则为null。
  - blockNumber: Number - 日志所在块的块号。如果是pending的日志，则为null。
  - address: String，32字节 - 日志产生的合约地址。
  - data: string - 包含日志一个或多个32字节的非索引的参数。
  - topics: String[] - 一到四个32字节的索引的日志参数数组。（在Solidity中，第一个主题是整个事件的签名（如，Deposit(address,bytes32,uint256)），但如果使用匿名的方式定义事件的情况除外）
事件监听器的返回结果，见后合约对象的事件。

示例：
```
var filter = web3.eth.filter('pending');

filter.watch(function (error, log) {
  console.log(log); 
  //  {"address":"0x0000000000000000000000000000000000000000", "data":"0x0000000000000000000000000000000000000000000000000000000000000000", ...}
});

// get all past logs again.
var myResults = filter.get(function(error, logs){ ... });

...

// stops and uninstalls the filter
filter.stopWatching();
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
