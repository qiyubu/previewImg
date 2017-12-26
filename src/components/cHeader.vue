<template>
  <div class="cHeader">
    <div class="cHeaderConWrap">
      <div class="cHeaderCon">
        <!--<img src="../assets/images/logo1.png" alt="云学堂" style="margin-top: 20px;height: 40px;">-->
        <!-- <div class="cHeaderNav">
             <a href="http://cloudclass.h3c.com/">
                 <div class="navItem">
                     <span class="navItemLi">运营中心</span>
                 </div>
             </a>
             <a href="http://h3classwiki.h3c.com/wiki">
                 <div class="navItem"><span class="navItemLi">wiki手册</span></div>
             </a>
             <a href="http://zhiliao.h3c.com/questions/catesDis/778">
                 <div class="navItem"><span class="navItemLi">问答社区</span></div>
             </a>
             <a href="    http://www.h3c.com/cn/Service/Software_Download/H3Cloud/">
                 <div class="navItem"><span class="navItemLi">软件下载</span></div>
             </a>
         </div>-->
        <div class="nav">
          <router-link :to="{name:'index'}" active-class="active" exact>
            <div class="navIt">
              <span class="itLi">首页</span>
            </div>
          </router-link>
          <router-link :to="{path:'/list'}" active-class="active">
          <div class="navIt">
            <span class="itLi">共享课堂</span>
          </div>
          </router-link>
          <router-link :to="{name:'pptIndex'}" active-class="active">
            <div class="navIt" active-class="active">
              <span class="itLi">共享课件</span>
            </div>
          </router-link>
          <a href="http://class.h3c.com:8888/" target="_blank">
            <div class="navIt">
              <span class="itLi">智能黑板</span>
            </div>
          </a>
          <a href="http://cloudclass.h3c.com/" target="_blank">
            <div class="navIt">
              <span class="itLi">运营中心</span>
            </div>
          </a>
          <a href="http://h3classwiki.h3c.com/wiki" target="_blank">
            <div class="navIt">
              <span class="itLi">wiki手册</span>
            </div>
          </a>
          <a href="http://zhiliao.h3c.com/questions/catesDis/778" target="_blank">
            <div class="navIt">
              <span class="itLi">问答社区</span>
            </div>
          </a>
          <a href="http://www.h3c.com/cn/Service/Software_Download/H3Cloud/Catalog/H3Cloud_Class/H3Cloud_Class/" target="_blank">
            <div class="navIt">
              <span class="itLi">软件下载</span>
            </div>
          </a>
          <router-link :to="{name:'theme'}" active-class="active">
            <div class="navIt" active-class="active">
              <span class="itLi">主题</span>
            </div>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        data() {
            return {
                msg: 'Hello World!'
            }
        }
    }
</script>

<style scoped>

  .cHeader {
    position: fixed;
    top: 0;
    left: 0;
    height: 80px;
    width: 100%;
    background-color: white;
    border: 1px solid #d1d1d1;
    box-shadow: 2px 2px 2px rgba(0,0,0,0.3);
    z-index: 5;
    box-sizing: border-box;
  }

  .cHeaderConWrap {
    width: 1280px;
    margin-left: auto;
    margin-right: auto;
    position: relative;
    height: 100%;
  }

  .cHeaderCon {
    width: 1176px;
    margin-left: 52px;
    margin-right: 52px;
    position: relative;
    height: 100%;
  }

  .cHeaderNav {
    position: absolute;
    right: 0;
    top: 0;
    font-size: 0;
  }

  .navItem {
    display: inline-block;
    font-size: 14px;
    color: #ffffff;
    line-height: 80px;
    margin: 0px 7px;
    position: relative;
  }

  .navItemLi:hover {
    /*background-image: url("../assets/images/head-bt-select.png");*/
  }

  .navItemLi {
    /*background-image: url("../assets/images/head-bt-default.png");*/
    height: 34px;
    line-height: 34px;
    width: 98px;
    display: inline-block;
    text-align: center;
  }

  .conWrap {

    width: 1200px;
    margin: 110px auto 0;
  }

  .nav {
    height: 80px;
    line-height: 80px;
    position: absolute;
    right: 0;
    top:0;
    font-size: 0;
    padding-left: 80px;
  }

  .navIt {
    display: inline-block;
    font-size: 18px;
    height: 80px;
    line-height: 80px;
    padding: 0 10px;
    margin: 0 10px;
    box-sizing: border-box;
    cursor: pointer;
    color: black;
  }

  .navIt:hover {
    border-bottom: 3px solid #188eee;
    color: #188eee;
  }
  .active .navIt{
    border-bottom: 3px solid #188eee;
    color: #188eee;
    display: inline-block;
    box-sizing: border-box;
    height: 80px;
  }


</style>
