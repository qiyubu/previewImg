<template>
  <div class="footer" id="Bottom">
    <div class="footerCon">
      <p class="ti">H3C</p>
      <p>版权所有  2017新华三技术有限公司版权所有</p>
      <p>京ICP备09032636号</p>
    </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        msg: 'Hello World!'
      }
    }
  }
</script>

<style lang="scss" scoped>
  /*footer*/
  .footer {
    background: #3D5FAE;
    background-size: auto 100%;
    box-sizing: border-box;
    height: 240px;
    color: #fff;
    text-align: center;
    width: 100%;
    min-width: 1200px;
  }
  .footerCon{
    font-size: 14px;
    position: relative;
    color: white;
    line-height: normal;
    top: 20%;
    .ti{
      font-weight: bolder;
      font-size: 30px;
      margin-bottom: 20px;
    }
  }

</style>
