# vue-circular-progress

> A Vue.js project

## Build Setup

```bash
npm i circular-progress-vue
```

````javaScript
import circularProgress from 'circular-progress-vue'
Vue.use(circularProgress)
```

```vue
<template>
  <circularProgress
    :options="options"
    :value="value"
  />
</template>
<script>
export default{
  data(){
    return{
      options:{
        //圆弧宽度（px）
        srtokeWidth: 2.5,
        //正值时的颜色
        negativeColor: '#56D5E4',
        //负值时的颜色
        positiveColor: '#FFC358',
        //圆弧半径（px）
        radius: 15,
        //加载时动画延时（ms）
        durTime:200,
        //背景色/空值时的颜色
        emptyColor:'#EEEEEE',
        //角度( 360 - 圆弧的角度 = angle )
        angle:90,
      },
      value:0.4
    }
  }
}
</script>
````

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
