# web3.currentProvider

如果已经设置了Provider，则返回当前的Provider。这个方法可以用来检查在使用mist浏览器等情况下已经设置过Provider，避免重复设置的情况。

调用：
```
web3.currentProvider
```

返回值：
- `Object` - null 或 已经设置的Provider对象。

示例：
```
if(!web3.currentProvider)
    web3.setProvider(new web3.providers.HttpProvider("http://localhost:8545"));
```

教程推荐：

- [以太坊DApp实战开发入门](http://xc.hubwiz.com/course/5a952991adb3847553d205d1?affid=github7878)
- [去中心化电商DApp实战开发](http://xc.hubwiz.com/course/5abbb7acc02e6b6a59171dd6?affid=github7878)
