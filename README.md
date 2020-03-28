> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-comment-items-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-comment-items-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1380)

* [npm包](https://www.npmjs.com/package/hm-uniapp-comment-items-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-comment-items-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-comment-items-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群（群号30423559）：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末回复提醒卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmCommentItemsCard from '@/components/hm-comment-items-card/index.vue'
export default {
    components: { HmCommentItemsCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-comment-items-card :options="options"></hm-comment-items-card>
  </div>
</template>
<script>
import HmCommentItemsCard from '@/components/hm-components/hm-comment-items-card/index.vue'

export default {
  components: { HmCommentItemsCard },
  data() {
    return {
      options: {
          shopCreditLv1:
            '/static/hm-comment-items-card/images/img_25837_0_0.png',
          daysAgo: '3 days ago',
          info: '老王回复了您'
        }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>

```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| shopCreditLv1        | String  | -      | 头像                                                                 |
| daysAgo        | String  | -      | 时间                                                                   |
| info        | String  | -      | 信息                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-03-07)

* 完成第一个版本
