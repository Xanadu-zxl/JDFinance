<template lang="html">
    <Panel class="panel">
        <section class="content">
            <swiper :options="options">
                <swiper-slide>百万白条券免费送，速来领取！！ <em>></em> </swiper-slide>
                <swiper-slide>签到领流量，1元500M！<em>></em> </swiper-slide>
            </swiper>
        </section>
    </Panel>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'
import Panel from '../core/panel.vue'
export default {
  components: {
    Panel,
    swiper,
    swiperSlide
  },
  data () {
    return {
      options: {
        autoplay: true,
        loop: true,
        direction: 'vertical'
      }
    }
  }
}
</script>

<style scoped>
.swiper-slide {
  font-family: PingFangSC-Medium;
  font-size: 12px;
  color: #333;
}
em {
  color: #ddd;
  float: right;
  margin-right: 20px;
}

.content {
  margin-top: 4rem;
  height: 72px;
  line-height: 72px;
  overflow: hidden;
  padding-left: 178px;
  background: url(//m.jr.jd.com/spe/qyy/main/images/scroll_title_img.png) left
    top no-repeat;
}
</style>
