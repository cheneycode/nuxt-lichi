<template>
  <div>
    <!--头部-->
    <header class="header">
      <div class="head">
        <div class="logo">
          <h1><img src="~assets/img/index/image_home_logo@1x.png"></h1>
        </div>
        <div class="menu">
          <ul>
            <nuxt-link v-for="(item,index) in menuData" :key="index" :to="item.key">
              <li :class="[active===item.key?'active':'']">{{item.val}}</li>
            </nuxt-link>
          </ul>
        </div>
      </div>
    </header>
  </div>
</template>


<script>
  export default {
    data() {
      return {
        active: '/',
        menuData: [{
          key: '/',
          val: '首页'
        }, {
          key: '/products',
          val: '产品中心'
        }, {
          key: '/about',
          val: '关于我们'
        }, {
          key: '/contact',
          val: '联系我们'
        }]
      }
    },
    created() {
      this.active = this.$nuxt.$route.fullPath;
    }
  }
</script>

<style>
</style>
