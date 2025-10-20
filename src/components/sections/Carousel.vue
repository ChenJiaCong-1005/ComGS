<script>
import { Swiper, SwiperSlide} from 'swiper/vue';
import { Navigation, Pagination, Autoplay} from 'swiper/modules';
import 'swiper/css/bundle';

export default {
  components: {
      Swiper,
      SwiperSlide,
      Navigation,
      Pagination,
      Autoplay,
    },
  data() {
    return {
      modules: [
        Navigation,
        Pagination,
        Autoplay,
      ],
      // 选择要轮播的照片
      image_paths: [
        "./carousel/coffee_martini.mp4",
        "./carousel/cut_roasted_beef.mp4",
        "./carousel/discussion.mp4",
        "./carousel/flame_steak.mp4",
        "./carousel/sear_steak.mp4",
        "./carousel/trimming_test.mp4",
      ],
    }
  }
}
</script>

<template>
  <el-row justify="center">
    <el-col :span="24">
      <!-- 设置轮播图：循环播放、首张图序号、响应式、导航和分页、自动播放 -->
      <swiper
        :loop="true"
        :slidesPerView="1"
        :breakpoints="{
          600: {
            slidesPerView: 2,
          },
          800: {
            slidesPerView: 3,
          },
        }"
        :modules="modules"
        :navigation="{ 
          hideOnClick:true,
        }"
        :pagination="{ 
          hideOnClick:true,
          clickable:true, 
          type:'bullets' 
        }"
        :autoplay="{ 
          delay:5000,
          disableOnInteraction:false,
          pauseOnMouseEnter:true,
        }"
        >
        <swiper-slide v-for="path in video_paths" :key="path">
    <video
      :src="path"
      controls
      autoplay
      loop
      muted
      playsinline
      style="width: 100%; height: auto; object-fit: cover"
    ></video>
          <el-image :src="path"/>
        </swiper-slide>
      </swiper>
    </el-col>
  </el-row>
</template>
  
<style>

/* 设置Swiper风格 */
.swiper {
  --swiper-theme-color: white;
}

</style>
  
