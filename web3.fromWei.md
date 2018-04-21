# web3.fromWei

以太坊货币单位之间的转换。将以wei为单位的资金，转换为指定单位的数值：

调用：
```
web3.fromWei(number, unit)
```

参数：
- `number`：.	Number|String|BigNumber - 数字或BigNumber。
- `unit`：.	String - 单位字符串

货币单位可取值如下

-	kwei/ada
-	mwei/babbage
-	gwei/shannon
-	szabo
-	finney
-	ether
-	kether/grand/einstein
-	mether
-	gether
-	tether

返回值：

- `String|BigNumber` - 根据传入参数的不同，分别是字符串形式的字符串，或者是BigNumber。

示例：
```
var value = web3.fromWei('21000000000000', 'finney');
console.log(value); // "0.021"
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
