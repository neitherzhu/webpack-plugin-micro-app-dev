# webpack-plugin-micro-app-dev

> 开发子应用时，获取主应用的一些全局依赖库与样式

## Install

Using npm:

```sh
npm install --save-dev webpack-plugin-micro-app-dev
```
## Usage

在`webpack`的`plugins`中增加代码
```js
const MicroAppDev = require('webpack-plugin-micro-app-dev');

"plugins": [
  new MicroAppDev({
    mainAppUrl: 'https://baas.uban360.com/portal', // 主应用的地址，通过这个地址获取主应用中的全局js与css依赖
  })
]
```