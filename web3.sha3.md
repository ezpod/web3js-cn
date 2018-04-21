# web3.sha3

使用keccak-256哈希算法，计算给定字符串的哈希值。

调用：
```
web3.sha3(string, options)
```

参数：

- `string`·：	String - 传入的需要使用Keccak-256 SHA3算法进行哈希运算的字符串。
-  `options`：	Object - 可选项设置。如果要解析的是hex格式的十六进制字符串。需要设置encoding为hex。因为JS中会默认忽略0x。

返回值：

- `String` - 使用Keccak-256 SHA3算法哈希过的结果。

示例：
```
//省略初始化过程
var hash = web3.sha3("Some string to be hashed");
console.log(hash); 
var hashOfHash = web3.sha3(hash, {encoding: 'hex'});
console.log(hashOfHash); 
```
教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
