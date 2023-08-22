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
              <span>Premium Skinbooster</span>
              <h3>
                Amazing experience for skin <br />
                MINUEL Mimi Booster
              </h3>
              <p>
                미미부스터는 트라넥사믹 에씨드, 시스테인, 아미노산 콤플렉스,<br/>
클루타티온 등의 유효성분이 어두운 피부에 밝은 광채 효과를 <br/>
내는 데 도움을 주는 프리미엄 부스터로서,<br/>
일반 스킨부스터와는 달리 실제 피부과클리닉<br/> 
의료진의 임상 검증을 통하여 효과가 입증된 프리미엄 부스터입니다.<br/>

              </p>
            </div>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <div class="dodo_progress">
              <div class="progress_inner skillsInner___" data-value="95">
                <span
                  ><span class="label">스킨 톤업
</span>
                  <span class="number">95%</span></span>
                <div class="background">
                  <div class="bar">
                    <div class="bar_in"></div>
                  </div>
                </div>
              </div>
              <div class="progress_inner skillsInner___" data-value="35">
                <span
                  ><span class="label">피부장벽개선</span
                  ><span class="number">35%</span></span>
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
              <div class="progress_inner skillsInner___" data-value="25">
                <span
                  ><span class="label">스킨 리쥬비네이션</span
                  ><span class="number">25%</span></span>
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
  name: "Booster",
  mounted() {
    window.addEventListener("scroll", activeSkillProgress);
  },
};
</script>
