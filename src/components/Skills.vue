<template>
  <div class="aali_tm_section">
    <div class="aali_tm_skills">
      <div class="container">
        <div class="skills_inner">
          <div class="left wow fadeInLeft" data-wow-duration="1s">
            <div
              class="aali_tm_main_title"
              data-text-align="left"
              data-color="light"
            >
              <span>Our purpose is</span>
              <h3>
                미산은 고객과 함께합니다.<br />
                We Can Do
              </h3>
              <p>
                Misan networks는 정직한 진료, 고객 중심, 사회 공헌의 기본이념을 바탕으로<br/>
                고객과 함께 하는 아름다운 성공을 향한 여행을 위해 <br/>
                현재에 머무르지 않고 더 나은 서비스를 제공하도록 노력하겠습니다.
              </p>
            </div>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <div class="dodo_progress">
              <div class="progress_inner skillsInner___" data-value="100">
                <span
                  ><span class="label">국내 병의원 지점확장</span>
                  <span class="number">100%</span></span>
                <div class="background">
                  <div class="bar">
                    <div class="bar_in"></div>
                  </div>
                </div>
              </div>
              <div class="progress_inner skillsInner___" data-value="100">
                <span
                  ><span class="label">뷰티산업 제품개발/연구</span
                  ><span class="number">100%</span></span>
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
              <div class="progress_inner skillsInner___" data-value="100">
                <span
                  ><span class="label">네트워크 및 뷰티제품의 글로벌화</span
                  ><span class="number">100%</span></span>
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <span
        class="border moving_effect"
        data-direction="x"
        data-reverse="yes"
      ></span>
    </div>
  </div>
</template>

<script>
import { activeSkillProgress } from "../utils/utils";

export default {
  name: "Skills",
  mounted() {
    window.addEventListener("scroll", activeSkillProgress);
  },
};
</script>
