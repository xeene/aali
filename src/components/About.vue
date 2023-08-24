<template>
  <div class="aali_tm_section" id="about">
    <div class="aali_tm_about">
      <div class="about_inner">
        <div class="left">
          <div class="image">
            <img src="img/about/1-1.jpg" alt="" />
            <div class="main" data-img-url="img/about/1-1.jpg"></div>
            <span
              class="square moving_effect"
              data-direction="y"
              data-reverse="yes"
            ></span>
            <span class="border"
              ><span
                class="in moving_effect"
                data-direction="x"
                data-reverse="yes"
              ></span
            ></span>
          </div>
        </div>
        <div class="center">
          <div class="title wow fadeInUp" data-wow-duration="1s">
            <span class="small">About Me</span>
            <h3>I'm <span>MISAN</span></h3>
            <h3>Beauty <span>Networks</span></h3>
            <span class="subtitle">Based in Seoul, Korea</span>
          </div>
          <div
            class="text wow fadeInUp"
            data-wow-duration="1s"
            data-wow-delay="0.2s"
          >
            <p>
              <strong>Hi, My name is MISAN.</strong> Misan Co., Ltd. is a medical creator group specializing in hospital management support (MSO). 
              We constantly strive and challenge to make the world healthier and more beautiful by expanding into various beauty areas through research and development, 
              as well as medical business based on the know-how of operating the New Star Clinic network. 

            </p>
            <p>
              ㈜미산은 병원경영지원(MSO) 전문 메디컬 크리에디터 그룹입니다. 
              뉴스타의원 네트워크 운영 노하우를 바탕으로 한 메디컬 비즈니스 뿐만 아니라, 
              연구/개발을 통한 다양한 뷰티 영역으로의 확대로 세상을 더 건강하고 아릅답게 만들기 위해 끊임없이 노력하고 도전합니다.
            </p>
          </div>
          <div
            class="aali_tm_button wow fadeInUp"
            data-wow-duration="1.5s"
            data-wow-delay="0.2s"
          >
            <!-- <a href="img/cv/1.jpg" download>
              <span v-html="download"> </span> 
            </a> -->
            <a href="http://brand.newstarclinic.co.kr/" target="_blank">
              <span v-html="download"> </span> 
            </a>
          </div>
        </div>
        <div class="right">
          <div class="image">
            <img src="img/about/1-2.jpg" alt="" />
            <div class="main" data-img-url="img/about/1-2.jpg"></div>
            <div
              class="square moving_effect"
              data-direction="x"
              data-reverse="no"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import { download } from "./svgImage";
export default {
  name: "About",
  data() {
    return {
      // download: `Download CV ${download}`,
      download: `Go, Medical Brand`
    };
  },
};
</script>
