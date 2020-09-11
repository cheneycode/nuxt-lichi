<template>
  <div>
    <page-header></page-header>
    <page-nav>
      <img src="~assets/img/product-center/image_product_pic_1.png" />
    </page-nav>
    <page-section>
      <!--品牌介绍部分-->
      <section class="container" style="margin-top: 100px;">
        <div class="content">
          <!--导航条-->
          <div class="navigation">
            <nuxt-link to="/">你的位置：首页 > </nuxt-link> 产品详情
          </div>
          <!--产品详情-->
          <div class="products-items">
            <div class="figure">
              <img class="img" :url="'/static/'+item.url">
            </div>
            <div class="info">
              <h2 class="name">{{item.name}}</h2>
              <h3 class="dsc">{{item.dsc}}</h3>
              <hr class="hr">
              <div class="info-list" v-for="(item,index) in item.infos " :key="index">
                <div class="info-key">
                  {{item.key}}
                </div>
                <div class="info-val">
                  {{item.val}}
                </div>
              </div>
            </div>
          </div>
          <!--商品详情-->
          <div class="products-item-img">
            <div class="products-item-title">
              <div class="det-name">
                商品详情
              </div>
            </div>
            <div class="det-imgs"></div>
          </div>
        </div>
      </section>
    </page-section>
    <page-footer></page-footer>
  </div>
</template>

<script>
  import axios from 'axios';
  export default {
    async asyncData({
      params
    }) {
      const app = await axios.get(`/data.json`)
      return {
        dataSource: app.data.data
      }
    },
    data() {
      return {
        dataSource: [],
        index: 0,
        item: {}
      }
    },
    created() {
      this.index = this.$nuxt.$route.params.id;
      this.item = this.dataSource[this.index];
      console.log(this.item)
    }
  }
</script>

<style>

</style>
