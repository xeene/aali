<template>
  <div class="aali_tm_section" id="blog">
    <div class="aali_tm_news">
      <div class="container">
        <div
          class="aali_tm_main_title"
          data-text-align="center"
          data-color="dark"
        >
          <span>개원진행 Q&A</span>
          <h3>아름다운 성공을 위해<br>함께 동행하시겠습니까?
</h3>
          <p>Will you accompany us to beautiful success?</p>
        </div>
        <div class="news_list">
          <ul>
            <li class="wow fadeInLeft" data-wow-duration="1s">
              <div class="list_inner">
                <div class="image">
                  <img src="img/blog/1.jpg" alt="" />
                  <div class="main" data-img-url="img/blog/1.jpg"></div>
                  <a
                    class="aali_tm_full_link"
                    @click.prevent="active = 1"
                    href="#"
                  ></a>
                </div>
                <div class="details">
                  <span class="category"
                    ><a href="#" @click.prevent="active = 1"
                      >Question</a
                    ></span
                  >
                  <h3 class="title">
                    <a href="#">개원위치 분석은 어떻게 하나요? 개원 기준은 어떻게 되나요?</a>
                  </h3>
                  <!-- <span class="date">November 10, 2021</span> -->
                </div>
                <div class="button">
                  <div class="aali_tm_learn_more">
                    <a href="#" @click.prevent="active = 1">Answer</a>
                  </div>
                </div>
                <div :class="`${active === 1 ? '' : 'news_hidden_details'}`">
                  <ModalBox :close="close">
                    <div class="news_popup_informations">
                      <div class="image">
                        <img src="img/blog/1.jpg" alt="" />
                        <div
                          class="main"
                          data-img-url="img/blog/1.jpg"
                          style="background-image: url('img/blog/1.jpg')"
                        ></div>
                      </div>
                      <div class="details">
                        <!-- <span class="category"><a href="#">Web Design</a></span> -->
                        <h3 class="title">
                          개원위치/상권 분석은 어떻게 하나요?
                        </h3>
                        <!-- <span class="date">November 10, 2021</span> -->
                        <div></div>
                      </div>
                      <div class="text">
                        <p>
                          - 개원하고자 하는 지역과 물건이 결정되면, 주변 메디컬 경쟁 상권 분석, 부동산 전문가를 통한 입지분석, 
                          성장 잠재력 등의 종합적 분석을 통해 의견을 드립니다.<br/>
                          - 개원준비 기간 동안 원장님들께서 처음 접해보는 일들에 관해 전문적 분석 및 제안을 드리고 개원 이후에는
                          경영컨설팅을 통해 병원의 수익구조의 개선부터 직원관리 및 교육 등의 분야에 관한 제안을 드리고 있습니다.
                        </p>
                        <p>
                          <strong>
                            향후 시장상황은 점점 경쟁이 심화되어, 개원 초기의 리스크 관리가 점점 더 중요합니다,
                            (주변 의료수가/고객군을 고려하지 않은 상품구성 및 장비 구매, 검증되지 않은 마케팅 투자, 섣부른 오퍼레이팅 인력관리 등)
                            이제는 개별 의료기관의 집중된 투자와 동시에, 공동의 관리 영역에서는 리스크의 분산 투자의 안목이 필요한 시대입니다. 
                          </strong>
                        </p>
                        <p class = "empty"></p>
                      </div>
                      <div class="details">
                        <h3 class="title">
                          개원 기준은 어떻게 되나요?
                        </h3>
                      </div>
                      <div class="text">
                        <p><strong>
                          - 대상 : 뉴스타 클리닉 개원 가능한 원장님(미용클리닉 경력 우대) <br/>
                          - 면적 : 전용면적 70평 이상 권장, 주차 여건 및 고객 접근이 용이한 상업지역 내<br/>
                          - 지역 : 서울, 수도권, 지방광역시 내 주요상업지역<br/>
                        </strong></p>
                        <p>
                          상기와 같은 기준은 필수 사항은 아나며 권장사항입니다. 다년간의 운영결과 원내 레이아웃, 고객 동선, 
                          장비배치 등을 고려하였을때 개원이후 불필요한 확장검토에 따른 이중비용지출방지, 면적대비 매출등을 
                          종합적으로 고려한 최소한의 기준입니다. 자세한 내용은 개원위치에 따른 검토후 협의와 검토를 통해 결정됩니다.
                        </p>
                      </div>
                    </div>
                  </ModalBox>
                </div>
              </div>
            </li>
            <li class="wow fadeInRight" data-wow-duration="1s">
              <div class="list_inner">
                <div class="image">
                  <img src="img/blog/4.jpg" alt="" />
                  <div class="main" data-img-url="img/blog/4.jpg"></div>
                  <a
                    class="aali_tm_full_link"
                    href="#"
                    @click.prevent="active = 2"
                  ></a>
                </div>
                <div class="details">
                  <span class="category"
                    ><a href="#" @click.prevent="active = 2"
                      >Question</a
                    ></span
                  >
                  <h3 class="title">
                    <a href="#" @click.prevent="active = 2"
                      >개원 후 운영관리는 어떻게 하나요? 뷰티 산업 동반성장은 어떻게 이뤄지나요?
</a
                    >
                  </h3>
                  <!-- <span class="date">October 22, 2021</span> -->
                </div>
                <div class="button">
                  <div class="aali_tm_learn_more">
                    <a href="#" @click.prevent="active = 2">Answer</a>
                  </div>
                </div>
                <div :class="`${active === 2 ? '' : 'news_hidden_details'}`">
                  <ModalBox :close="close">
                    <div class="news_popup_informations">
                      <div class="image">
                        <img src="img/blog/4.jpg" alt="" />
                        <div
                          class="main"
                          data-img-url="img/blog/4.jpg"
                          style="background-image: url('img/blog/4.jpg')"
                        ></div>
                      </div>
                      <div class="details">
                        <!-- <span class="category"
                          ><a href="#">Development</a></span
                        > -->
                        <h3 class="title">
                          <a href="#">개원 후 운영관리(Operating)는 어떻게 하나요?</a>
                        </h3>
                        <!-- <span class="date">October 22, 2021</span> -->
                        <div></div>
                      </div>
                      <div class="text">
                        <p>
                          - 경력 10년 이상의 전문 운영관리 인원이 개원 확정부터 개원 이후까지 전문적인 노하우를 공유합니다.
<br/>
                        - 개원 이후에도 소통의 장이 되고자 시술정보 및 경영정보 컨퍼런스를 진행하고 있습니다. 정기적, 분기별로 온.오프라인 컨퍼런스, 세미나를 개최하여 네트워크 원장님들의 인적 교류와 전문성 강화를 돕고 있으며,. 컨퍼런스는 각 분야별 1등 전문가들을 초빙하여 강의, 질의 응답 상담 등이 진행 됩니다.
급변하는 의료시장에서 다양한 경험과 정확한 정보는 성공의 열쇠와 다름없습니다.
-차별화된 전략과 체계적인 시스템으로 병의원 개원과 경영에 관한 최고의 만족을 드리겠습니다.

                        </p>
                        <p><strong>‘브랜드’는 우리의 얼굴입니다. 브랜드 가치의 성장을 위해 끊임없는 노력을 추구합니다. 
</strong>
                        </p>
                        <p class = "empty"></p>
                      </div>
                      <div class="details">
                        <h3 class="title">
                          뷰티 산업 동반성장은 어떻게 이뤄지나요?
                        </h3>
                      </div>
                      <div class="text">
                        <p>
                         - Misan networks는 병원운영관리 뿐만 아니라 다양한 뷰티산업으로의 확대를 모색하고 있습니다.<br>
- 대부분의 네트워크가 본점 위주의 성장을 추구하나,  뉴스타 클리닉 네트워크는 원장님들과 동반성장의 길을 걷고자 합니다. Misan networks가 개발한 제품의 우선공급과 함께 향후 진행할 다양한 뷰티 제품의 연구/개발 참여를 통한 새로운 사업기회 모색, K-Beauty 산업의 해외 시장 공동 진출, 시대의 변화에 따른 다양한 메디컬 컨텐츠 개발 및 공유 등을 통해 차별화의 길을 걷고자 합니다. 

                        </p>
                        <p><strong>개원이후 지점 단순관리에 안주하지 않고, 꾸준한 성장을 함께 고민해 나가는 네트워크가 되고자 합니다.</strong>
                        </p>
                      </div>

                    </div>
                  </ModalBox>

                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ModalBox from "./ModalBox.vue";
export default {
  name: "Blog",
  data() {
    return {
      active: 0,
    };
  },
  methods: {
    close() {
      this.active = 0;
    },
  },
  components: { ModalBox },
};
</script>
