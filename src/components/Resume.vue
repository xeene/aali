<template>
  <div class="aali_tm_section">
    <div class="aali_tm_resume">
      <div class="content">
        <div class="container">
          <div class="resume_in">
            <div class="aali_tm_main_title" data-text-align="left" data-color="dark">
              <span>Know More</span>
              <h3>Our Main History </h3>
              <!-- <p>
                I enjoy every step of the design process, from discussion and
                collaboration to concept and execution
              </p> -->
            </div>
            <div class="content_inner">
              <ul>
                <li class="wow fadeInLeft" data-wow-duration="1s">
                  <h3 class="main_title"><span>Misan Co.</span></h3>
                  <ul class="list">
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2022</h3>
                            <!-- <span>University of Maine</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2018 - 2020</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            01月 ‘미미부스터‘ 연구 및 개발 시작<br />12月 ‘미미부스터‘ 임상 테스트 결과 성공

                          </p>
                        </div>
                      </div>
                    </li>
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2023</h3>
                            <!-- <span>University of Texas</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2014 - 2018</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            02月 주식회사 미산 설립<br />
                            04月 뉴스타의원 성수점 개원<br />
                            07月 ‘미미부스터’ 출시 성공<br>
                            국내 및 해외 병원 다수 입점

                          </p>
                        </div>
                      </div>
                    </li>
                    <li>
                      <div class="list_inner">
                        <div class="wrapper">

                          <div class="aali_tm_button border">
                            <a class="aali_tm_full_link" href="#" @click.prevent="active = 1"><span
                                v-html="`MISAN Client`"></span></a>
                          </div>
                        </div>

                      </div>
                    </li>
                    <div :class="`${active === 1 ? '' : 'resume_hidden_details'}`">
                      <ModalBox :close="close">
                        <div class="resume_popup_informations">
                          <!-- <div class="image">
                            <img src="img/thumbs/4-2.jpg" alt="" />
                            <div class="main" data-img-url="img/service/4.jpg"
                              style="background-image: url('img/service/4.jpg')"></div>
                          </div> -->
                          <swiper 
                            class="owl-carousel ul reSwiper"
                            :options="swiperOptions"
                            ref="resumeSwiper"
                          >
                            <swiper-slide class="item li">
                              <div class="re_img">
                                <img src="img/cv/worldwide.jpg">
                              </div>
                            </swiper-slide>
                            <swiper-slide class="item li">
                              <div class="re_img">
                                <img src="img/cv/local.jpg">
                              </div>
                            </swiper-slide>
                          </swiper>
                          <div class="resumeNav">
            <a class="prev_" href="#">❮</a>
            <a class="next_" href="#">❯</a>
          </div>
                        </div>
                      </ModalBox>
                    </div>

                  </ul>
                </li>
                <li class="wow fadeInRight" data-wow-duration="1s">
                  <h3 class="main_title"><span>Newstar Clinic</span></h3>
                  <ul class="list">
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2013~2014</h3>
                            <!-- <span>Easy Computers</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2018 - running</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            2013.8 US Galderma Korea 전문교육과정 이수<br />
                            2013.8 레스틸렌 EXPERT 키닥터<br />
                            2013.9 KPCS Laser Academy Certificate<br />
                            2014.11 고객감동경영 & 스타의료인 브랜드 대상 수상<br />
                          </p>
                        </div>
                      </div>
                    </li>
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2015~2019</h3>
                            <!-- <span>eTheme Group</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2015 - 2018</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            2017.4 비만센터 오픈<br />
                            2018.9 소비자 만족 브랜드 대상 1위 수상<br />
                            2019.1 SINCLAIR 프리미엄 콜라겐센터 블랙라벨 지정<br />
                            2019.3 Inmode 키닥터<br />
                            2019.11 엑스퍼트(Xspurt)필러 키닥터

                          </p>
                        </div>
                      </div>
                    </li>
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2020~2022
                            </h3>
                            <!-- <span>Envato Studio</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2012 - 2018</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            2020.2 한국범죄심리학회 협력위원회 위원임명<br />
                            2022.8 Alma SINON∥ 루비레이저 공식인증 클리닉<br />
                            2022.9 뉴욕 CLEAR LASER CLINIC Dr. 참관 교육<br />
                            2022.10 휴젤 THE CHAEUM 필러 명예의전당 수상<br />
                            2022.11 티타늄리프팅 공식인증 클리닉

                          </p>
                        </div>
                      </div>
                    </li>
                    <li>
                      <div class="list_inner">
                        <span class="icon" v-html="exp"></span>
                        <div class="info">
                          <div class="left">
                            <h3>2023</h3>
                            <!-- <span>Envato Studio</span> -->
                          </div>
                          <!-- <div class="right">
                            <span>2012 - 2018</span>
                          </div> -->
                        </div>
                        <div class="text">
                          <p>
                            2023.1 쥬베룩 정품 시술 병원 인증<br />
                            2023.4 뉴스타의원 성수점 오픈<br />
                            2023.5 Onda 키닥터
                          </p>
                        </div>
                      </div>
                    </li>
                  </ul>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="media" data-background-style="video">
        <!-- Background Styles: "video" and "image" // Also you can use any youtube, vimeo, and local videos https://vimeo.com/337293658 https://www.youtube.com/watch?v=9BMR3y7RLpc-->
        <div class="video jarallax" data-speed="0" data-jarallax-video="https://vimeo.com/856354378"></div>
        <div class="image jarallax" data-speed="0" data-img-url="img/about/2.jpg"></div>
        <span class="square moving_effect" data-direction="y" data-reverse="yes"></span>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import ModalBox from "./ModalBox.vue";
import { jarallaxContent } from "../utils/utils";
import { edu, exp } from "./svgImage";

export default {
  name: "Resume",
  data() {
    return {
      edu,
      exp,
      active: 0,
      swiperOptions: {
        slidesPerView: 1,
        loop: true,
        pagination: false,
        navigation: {
          prevEl: ".prev_",
          nextEl: ".next_",
        },
        autoplay: true
      },

    };
  },
  mounted() {
    jarallaxContent();
  },
  methods: {
    close() {
      this.active = 0;
    },
  },
  components: { ModalBox, Swiper, SwiperSlide },
  computed: {
    siper() {
      return this.$refs.resumeSwiper.$swiper
    },
  },

};
</script>
