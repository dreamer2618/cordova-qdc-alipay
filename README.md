# cordova-qdc-alipay
支付宝APP支付cordova,ionic插件(Android版，IOS版)

* 2015.07.02 IOS版支付宝集成
* 2015.07.02 支付宝签名算法移至服务端
* 2015.07.01 支付宝Android集成，初步完成
* 2016.09.13 android,ios sdk更新为当前版本:android:v15.2.2 ios v15.2.0
## 1.1 JS调用说明

* 事先前调用后台服务端API生成订单数据及签名数据
* 调用plugin的JS方法【alipay.payment】进行支付

```js
	**alipay.payment(json, cb_success, cb_failure);**
	# 参数说明：格式为JSON格式
	# cb_success:调用成功回调方法
	# cb_failure:调用失败回调方法
	# json: {
	    pay_info: 支付信息
	    sign: 密钥
	  }
```

