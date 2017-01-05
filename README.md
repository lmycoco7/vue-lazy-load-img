## 关于
本插件基于[lazy-load-img](https://github.com/lzxb/lazy-load-img)的vue版本实现，请到[lazy-load-img](https://github.com/lzxb/lazy-load-img)查看文档

## 支持AMD、CMD、和页面直接引入使用，下面只列出CMD的使用教程
```javascript
// npm install --save-dev lazy-load-img 
// npm install --save-dev vue-lazy-load-img

import Vue from 'vue'
import VueLazyLoadImg from 'vue-lazy-load-img'

Vue.use(vue-lazy-load-img)

```
```vue
<vue-lazy-load-img 
    mode="diy"
    :time="300"
    :complete="true"
    :position="{ top: 0, right: 0, bottom: 0, left: 0 }"
    :diy="{ backgroundSize: 'cover', backgroundRepeat: 'no-repeat', backgroundPosition: 'center center' }"
    @before="before" 
    @success="success" 
    @error="error">
    <img src="./images/default.png" data-src="./images/test.png" alt="">
</vue-lazy-load-img>
```
