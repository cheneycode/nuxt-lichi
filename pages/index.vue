<template>
  <div>
    <page-header></page-header>
    <page-nav>
      <img src="~assets/img/index/image_home_banner.png" />
    </page-nav>
    <page-section>
      <!--品牌介绍部分-->
      <section class="container">
        <div class="content">
          <!--品牌介绍部分-->
          <div class="brand-item">
            <div class="item-text">
              <h1>公司介绍 ---</h1>
              <div class="brand-item-text">
                北京励齿医疗科技有限公司（简称“励齿”）创立于2016年初，是由日本森田公司、日进公司、台湾FOMED公司等口腔行业知名企业与上海投资成立。我们拥有口腔业界经验丰富的专业团队，励齿经营产品涵盖口腔行业全系列产品。<br><br>
                业绩顶尖的商品数量、全方位的口腔产品采购咨询/指导、快捷/稳健的物流支撑、专业帖贴心的售前/售后服务、证件齐备及全正品保障。目前和国内外100多个知名品牌厂商建立深度合作关系，为您专业提供牙科器械、材料、设备、制服等全品类口腔医疗产品，以优质的产品和完善的服务。
              </div>
            </div>
          </div>
          <div class="brand-image">
            <img src="~assets/img/index/image_home_brand.png">
          </div>
          <!--产品中心部分-->
          <div class="products-item">
            <div class="item-title">
              >> 产品中心
            </div>
            <div class="products-list">
              <div class="list-item" @click="linkDetil(0)" data-type="0">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_1.png">
                </div>
                <div class="list-text">
                  <h2 class="active">根管测量仪器</h2>
                  <h4>八颗牙 | 根管测量仪器</h4>
                </div>
              </div>
              <div class="list-item" @click="linkDetil(1)" data-type="1">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_2.png">
                </div>
                <div class="list-text">
                  <h2>#RelyX Ultimate树脂水门汀（绿巨人）</h2>
                  <h4>3M ESPE|RelyX Ultimate树脂水门汀（绿巨人）</h4>
                </div>
              </div>
              <div class="list-item" @click="linkDetil(2)" data-type="2">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_3.png">
                </div>
                <div class="list-text">
                  <h2>美佳印咬合记录硅橡胶</h2>
                  <h4>沪鸽 | 美佳印®咬合记录硅橡胶</h4>
                </div>
              </div>
              <div class="list-item" @click="linkDetil(3)" data-type="3">
                <div class="list-box">
                  <img src="~assets/img/index/image_home_product_4.png">
                </div>
                <div class="list-text">
                  <h2>T3 Boost 快接式涡轮手机</h2>
                  <h4>西诺德 | T3 快接式涡轮手机</h4>
                </div>
              </div>
              <div class="list-item" @click="linkDetil(4)" data-type="4">
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
          <!--联系我们部分-->
          <div class="contactus-item">
            <div class="item-title">
              >> 联系我们
            </div>
            <div class="contactus-map">
              <img src="~assets/img/index/image_home_map.png">
            </div>
            <div class="contactus-text">
              <h2>公司名称：北京励齿医疗科技有限公司</h2>
              <h2>联系电话：400-810-6692</h2>
              <h2>联系地址：北京市通州区中关村科技园区通州园金桥科技产业基地景盛南二街10号院10号楼八层802</h2>
            </div>
          </div>
        </div>
      </section>
    </page-section>
    <page-footer></page-footer>
  </div>
</template>

<script>
  export default {
    data() {
      return {

      }
    },
    created() {

    },
    methods: {
      linkDetil(index) {
        this.$nuxt.$router.push(`/products/${index}`)
      }
    }
  }
</script>

<style>

</style>
