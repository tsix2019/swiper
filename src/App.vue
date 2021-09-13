<template>
  <div>
    <swiper>
      <SwiperItem v-for="(item, index) in goods" :key="index">
        <a :href="item.link">
          <img :src="item.image" alt="" />
        </a>
      </SwiperItem>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperItem } from "./components/swiper/index";
export default {
  data() {
    return {
      goods: [
        { link: "https://www.mi.com", image: "https://s3.bmp.ovh/imgs/2021/09/1cb4db872ddb0e17.jpg" },
        { link: "https://www.mi.com", image: "https://s3.bmp.ovh/imgs/2021/09/1cb4db872ddb0e17.jpg" },
        { link: "https://www.mi.com", image: "https://s3.bmp.ovh/imgs/2021/09/1cb4db872ddb0e17.jpg" },
        { link: "https://www.mi.com", image: "https://s3.bmp.ovh/imgs/2021/09/1cb4db872ddb0e17.jpg" },
      ],
    };
  },
  components: {
    Swiper,
    SwiperItem,
  },
};
</script>

<style scoped>
  SwiperItem{
    height: 300px;
  }
</style>