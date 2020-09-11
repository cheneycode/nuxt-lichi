<template>
  <div>
    <page-header></page-header>
    <page-nav>
      <img src="~assets/img/product-center/image_product_pic_1.png" />
    </page-nav>
    <page-section>
      <!--品牌介绍部分-->
      <section class="container">
        <div class="content">
          <!--导航条-->
          <div class="navigation">
             <nuxt-link to="/">你的位置：首页 > </nuxt-link> 产品中心
          </div>
          <!--产品中心部分-->
          <div class="products-item" style="margin-top: 50px;">
            <div class="item-title">
              产品中心
            </div>
            <div class="products-list">
              <div class="list-item" data-type="0">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_1.png">
                </div>
                <div class="list-text">
                  <h2 class="active">根管测量仪器</h2>
                  <h4>八颗牙 | 根管测量仪器</h4>
                </div>
              </div>
              <div class="list-item" data-type="1">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_2.png">
                </div>
                <div class="list-text">
                  <h2>#RelyX Ultimate树脂水门汀（绿巨人）</h2>
                  <h4>3M ESPE|RelyX Ultimate树脂水门汀（绿巨人）</h4>
                </div>
              </div>
              <div class="list-item" data-type="2">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_3.png">
                </div>
                <div class="list-text">
                  <h2>美佳印咬合记录硅橡胶</h2>
                  <h4>沪鸽 | 美佳印®咬合记录硅橡胶</h4>
                </div>
              </div>
              <div class="list-item" data-type="3">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_4.png">
                </div>
                <div class="list-text">
                  <h2>T3 Boost 快接式涡轮手机</h2>
                  <h4>西诺德 | T3 快接式涡轮手机</h4>
                </div>
              </div>
              <div class="list-item" data-type="4">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_5.png">
                </div>
                <div class="list-text">
                  <h2>PM700标准版无痛牙周超声治疗系统</h2>
                  <h4>EMS | PM700标准版无痛牙周超声治疗系统</h4>
                </div>
              </div>
              <div class="list-item" style="visibility: hidden;"></div>
            </div>
          </div>
        </div>
      </section>
    </page-section>
    <page-footer></page-footer>
  </div>
</template>

<script>
  export default {}
</script>

<style>

</style>
