<template>
  <div>
    <!--{{msg}}-->
    <mallHeader></mallHeader>
    <div class="imgWrap">
      <div class="imgTitle">
        主题下载
      </div>
      <BigImg :data="imgList"></BigImg>
    </div>
    <mallFooter></mallFooter>
  </div>
</template>

<script>
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
  }
</script>

<style lang="scss" scoped>
  .imgWrap{
    width: 1200px;
    margin: 0 auto;
    padding: 30px;
    min-height: 400px;
    box-sizing: border-box;
    .imgTitle{
      font-size: 24px;
      height: 40px;
      line-height: 40px;
    }
  }

</style>
