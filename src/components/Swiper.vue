<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
        <!-- slides -->
        <swiper-slide v-for="item of swiperList" :key="item.id"><img class="swiper-img" :src="item.imgUrl" /></swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
        <!-- 左右箭头 -->
        <!-- <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div> -->
        <!-- 底部滚动条 -->
        <!-- <div class="swiper-scrollbar"   slot="scrollbar"></div> -->
        </swiper>
    </div>
</template>


<script>
export default {
  name : 'HomeSwiper',
  data () {
      return {
          swiperOption: {
              pagination:'.swiper-pagination',
              loop: true
          },
          swiperList: [{
              id: '0001',
              imgUrl: 'http://img1.qunarzz.com/piao/fusion/1810/23/e24143794d9cbb02.jpg_890x330_9689bdd2.jpg'
          },{
              id: '0002',
              imgUrl: 'http://img1.qunarzz.com/piao/fusion/1809/b6/23980fda69a67d02.jpg_890x330_fe885a29.jpg'
          },{
              id: '0003',
              imgUrl: 'http://img1.qunarzz.com/piao/fusion/1809/91/836652a03cc5f802.jpg_890x330_628a9416.jpg'
          },{
              id: '0004',
              imgUrl: 'http://img1.qunarzz.com/piao/fusion/1706/6b/48f71452f4622c02.jpg_890x330_968f00af.jpg'
          }]
      }
  }    
}
</script>

<style scope>
  .wrapper >>> .swiper-pagination-bullet-action{
      background: #fff !important;
  }
  .wrapper{
      width:100%;
      overflow: hidden;
      height: 0;
      padding-bottom: 35%;
  }
  .swiper-img{
      width:100%;
      background: rgb(207, 202, 202);
  }
</style>
