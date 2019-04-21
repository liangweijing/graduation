<template>
    <div>       
<swiper class="swiper swiper-container" 
            :indicator-dots="true" 
            interval="5000" 
            duration="1000" 
            autoplay>
      <block v-for="(item, index) in imgUrls" :index="index" :key="index">
          <swiper-item>
              <img :src="item.src" class="swiper-slide" width="355" height="150"/>
          </swiper-item>
      </block>
    </swiper>
    <div style="height:150rpx;width:355rpx;border:1px solid red">
<image scr="/static/images/swiper2.jpg" class="slide-image" />
    </div>

    </div>
</template>
<script>
export default {
  data() {
      return {
 imgUrls: [
{src:'/static/images/swiper1.jpg'},
  {src:'/static/images/swiper2.jpg'}    ,
      {src:'https://images.unsplash.com/photo-1551446591-142875a901a1?w=640'}
    ],
      }
  }
}
</script>
