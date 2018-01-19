<template>
  <div class="box">
   <!-- 顶部导航 -->
    <navheader></navheader>
    <!-- 商品系列导航 -->
    <navlist></navlist>
    <div class="des-main">
      <p class="bread"><span>健康食品</span><b>></b><span>婴幼儿食品</span><b>></b><span>a2 白金婴儿配方幼儿奶粉...</span></p>
      <div class="lunbo">
        <div class="lun-l">
          <div class="lun-l-top">
            <img src="../../assets/images/g1.jpg" alt="">
          </div>
          <div class="lun-l-bottom"></div>
        </div>
        <div class="lun-r">
          <p class="l-tit">a2 白金婴儿配方幼儿奶粉三段 900克/罐 4罐 1-3岁</p>
          <div class="lun-price">
            <p><span>售价</span><b class="lun-native">$170</b><em>/</em><span class="lun-vip">我的会员价:</span><b class="lun-native">$160</b></p>
            <p><span>汇率</span><span class="huilu">5.0704</span></p>
          </div>
          <div class="lun_mes">
            <p><span id="ways">物流方式</span><span class="huoji samew">国际物流</span><span class="samew shang">上门自提</span></p>
            <p><span>重量</span><span>4.52kg</span></p>
            <p><span>数量</span><span><el-input-number size="small" v-model="num6"></el-input-number></span></p>
            <p><span>说明</span><span>不支持使用优惠券</span></p>
          </div>
          <p><button class="nowpay">立即购买</button><button class="addcar">加入购物车</button><span class="xing">☆</span><span class="star">收藏</span></p>
        </div>
      </div>
      <!-- 详情 评价 参数介绍 -->
      <div class="detail-main"></div>
    </div>
     <!-- 底部介绍 -->
    <footlist></footlist>
  </div>
</template>

<script>
 export default {
    name: 'description',
    components: {
        
    },
    data() {
     return {
        checked: true,
         num6: 1,
      };
    },
 
  }
</script>

<style scoped>
  .des-main {
    width:1200px;
    margin:0 auto;
  }
  /* 面包屑 */
    .bread {
      height: 57px;
      line-height: 57px;
      width:100%;
      font-size:16px;
    }
    .bread b {
      margin:0 10px;
    }
  /* 轮播图部分 */
    .lunbo {
      width: 100%;
      height:535px;
    }
    /* 左边 图片盒子 */
    .lun-l {
      width:440px;
      height: 535px;
      border:1px solid #ccc;
      float:left
    }
    .lun-l-top {
      width:100%;
      height:410px;
    }
    .lun-l-top img {
      width:100%;
      height:408px;
    }
    /* 右边盒子 */
    .lun-r {
      float:left;
      width:730px;
      margin-left:30px;
    }
    .l-tit {
      font-size:28px;
      padding-left: 15px;
    }
    .lun-price {
      background-color: #fafafa;
      margin-top:20px;
      padding-left: 15px;
    }
    .lun-price p {
      height:44px;
      line-height:44px;
      font-size:16px;
    }
    .lun-price span {
      display: inline-block;
    }
    .lun-r p span:first-child {
      letter-spacing: 32px;
      width:120px;
    }
    .lun-native {
      display: inline-block;
      color:#d4282d;
      font-size:28px;
    }
    .lun-price p em {
      font-size:28px;
      margin:0 10px;
    }
    .lun-vip {
      margin-right:10px;
      font-size:14px;
      vertical-align: middle;
    }
    .huilu {
      height: 20px;
      border:1px solid #d4282d;
      line-height: 12px;
      font-size:14px;
      padding:4px; 
    }
    .lun_mes {
      padding-left: 15px;
      font-size:16px;
      border-bottom:1px solid #eee;
      margin-bottom:20px;
      margin-top:20px;
    }
    .lun_mes #ways {
      display:inline-block;
      letter-spacing: 0px;
      width:120px;
    }
    .lun-r .lun_mes span:first-child {
      display:inline-block;
      width:120px;
    }
    .lun_mes p {
      height: 50px;
      line-height:50px;
    }
    .samew {
      border:1px solid #ccc;
      display:inline-block;
      width: 110px;
      height: 40px;
      line-height:40px;
      text-align: center;
    }
    .huoji {
      border:1px solid #d4282d;
      color:#d4282d;
      margin-right:20px;
    }
    .lun-r button {
      width: 200px;
      height:70px;
      font-size:28px;
      outline: none;
    }
    .nowpay {
      border:2px solid #d4282d;
      color:#d4282d;
      margin-right:20px;
    }
    .addcar {
      background: #d4282d;
      color:#fff;
    }
    .xing {
      font-size: 35px;
      color:#d4282d;
      height:70px;
      line-height:70px;
      display:inline-block;
      vertical-align: top;
      margin-left:25px;
      margin-right:10px;
    }
    .star {
      font-size:18px;
      height:70px;
      line-height:70px;
      display:inline-block;
      vertical-align: top;
    }

  /* 详情 评价 参数介绍 */
  .detail-main {
    width:100%;
    height:800px;
    border:1px solid red;
  }
</style>


