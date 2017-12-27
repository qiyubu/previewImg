# preview_imgs

> js preview images 

vue 2.5.2 版本 vue组件
实现点击预览大图功能，点击下载图片功能（不兼容IE，适用于PC端）
内部代码可实现点击图片旋转效果，在本处无用，故注释掉，如有需要可打开调整

# 使用方法
``` bash
<BigImg :data="imgList"></BigImg>

 import BigImg from '../components/previewImg.vue'
  import mallHeader from '../components/cHeader.vue'
  import mallFooter from '../components/cFooter.vue'

  export default {
    data () {
      return {
        imgList: [
          {path: 'http://ppt.h3c.com:5005/static/img/theme/theme1.jpg'},
          {path: 'http://ppt.h3c.com:5005/static/img/theme/theme2.jpg'},
          {path: 'http://ppt.h3c.com:5005/static/img/theme/theme3.jpg'}
        ]
      }
    },
    components: {
      BigImg,
      mallHeader,
      mallFooter
    }
    ```


For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
