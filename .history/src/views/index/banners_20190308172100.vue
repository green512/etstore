<template>
  <div class="banner-warp">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item in banners" :key="item.goods">        
        <router-link :to="'/app/home/productDetail/'+item.goods" target = _blank> <img :src="item.image" alt="" /></router-link>
        <div class="title"> {{item.title}}</div>
        <div class="content"> {{item.content}}</div>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>
<style>
  .banner-warp{
    display: inline;
  }
  .banner-warp img{
    width: 100%;
 }
 .title{
   border-width: 0px;
    position: absolute;
    left: 495px;
    top: 60px;
    width: 564px;
    height: 57px;
    font-family: 'Times New Roman Negreta', 'Times New Roman Normal', 'Times New Roman';
    font-weight: 700;
    font-style: normal;
    font-size: 48px;
    color: #faf6f6;
 }
 .content{
    border-width: 0px;
    position: absolute;
    left: 261px;
    top: 305px;
    width: 871px;
    height: 29px;
    font-family: 'Arial Negreta', 'Arial Normal', 'Arial';
    font-weight: 700;
    font-style: normal;
    font-size: 24px;
    color: #363636;
}
</style>



<script>
  import { swiper, swiperSlide } from 'vue-awesome-swiper'
  import {bannerGoods} from '../../api/api'

  export default {
    components: {
      swiper,
      swiperSlide,
    },
    data() {

      return {

        swiperOption: {
          pagination: '.swiper-pagination',
          paginationClickable: true,
          autoplay: 2500,
          autoplayDisableOnInteraction: false,
        },
        banners:[]

      }

    },
    methods:{
      getBanner(){
        bannerGoods()
          .then((response)=> {
            console.log(response)
            //跳转到首页页response.body面
            this.banners = response.data
          })
          .catch(function (error) {
            console.log(error);
          });
      }
    },
    created(){
      this.getBanner();
    }

  }

</script>
