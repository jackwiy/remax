---
title: 小程序 API
order: 26
---

Remax 提供原生小程序 API 支持，如；

```js
import { navigateTo, requestPayment, ... } from 'remax/wechat'
```

拥有事件回调（success，fail）的 API，Remax 还提供 `Promise` 支持，如：

```js
import { requestPayment } from 'remax/wechat';

requestPayment(params).then(res => {
  console.log(res);
});
```

如果你需要直接访问原生 api，或者需要使用 remax 还没有更新的 api，也可以直接访问原生模块：

```js
import { native } from 'remax/wechat';

// native 相当于微信小程序中的 wx 变量
```
