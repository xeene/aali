<template>
  <div class="aali_tm_section" id="testimonial">
    <div class="aali_tm_testimonials helpMob">
      <div class="left">
        <div class="image">
          <img src="img/hero/1.png" alt="" />
        </div>
      </div>
      <div class="right">
        <div class="right_in">
          <div
            class="aali_tm_main_title"
            data-text-align="left"
            data-color="light"
          >
            <span>MINUEL Mimi Booster</span>
            <h3>스킨 톤업 효과에 집중
</h3>
          </div>
          <swiper
            class="owl-carousel ul"
            :options="swiperOptions"
            ref="mySwiper"
          >
            <swiper-slide class="item li">
              <div class="text">
                <p>
                 <!-- <img src="img/thumbs/test.gif" alt=""> -->
                 <!-- ^это должно масштабироваться в мобильной версии как-тo; убрать паддинг топ если будет 400 -->
                </p>
              </div>
              <div class="name">
                <h3><span>자체시험결과/ 원료적 특성에 한함</span></h3>
              </div>
            </swiper-slide>
            <swiper-slide class="item li">
              <div class="text">
                <p>
                 Картинка
                </p>
              </div>
              <div class="name">
                <h3><span>한국 내 병원과 자체협약, 임싱실험 진행결과</span></h3>
              </div>
            </swiper-slide>
            <swiper-slide class="item li">
              <div class="text">
                <p>
Картинка
                </p>
              </div>
              <div class="name">
                <h3><span>자체시험결과/ 원료적 특성에 한함</span></h3>
              </div>
            </swiper-slide>
            <swiper-slide class="item li">
              <div class="text">
                <p>
Картинка
                </p>
              </div>
              <div class="name">
                <h3>MacLaren, <span>Freelancer</span></h3>
              </div>
            </swiper-slide>
          </swiper>
          <div class="direct">
            <a class="prev_button" href="#"><i class="icon-left"></i></a>
            <a class="next_button" href="#"><i class="icon-right"></i></a>
          </div>
        </div>
      </div>
      <span class="border"
        ><span
          class="in moving_effect"
          data-direction="x"
          data-reverse="yes"
        ></span
      ></span>
      <span
        class="square moving_effect"
        data-direction="y"
        data-reverse="yes"
      ></span>
      <span class="quote moving_effect" data-direction="x"
        ><i class="icon-quote-left"></i
      ></span>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
export default {
  name: "Testimonial",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      swiperOptions: {
        slidesPerView: 1,
        loop: true,
        pagination: false,
        navigation: {
          prevEl: ".prev_button",
          nextEl: ".next_button",
        },
      },
    };
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper;
    },
  },
};
</script>
