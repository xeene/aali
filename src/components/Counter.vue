<template>
  <div class="aali_tm_section">
    <div class="aali_tm_counter">
      <div class="container">
        <div class="counter_list">
          <ul class="wow fadeIn" data-wow-duration="1s">
            <li>
              <div class="list_inner">
                <div class="wrapper">
                  <div class="value">
                    <VisibilitySensor @change="onChange">
                      <span class="abs"
                        ><span class="tm_counter"
                          ><number
                            ref="tm_counterk"
                            :to="10000"
                            animationPaused
                            :duration="3"
                          /> </span
                        ><label class="small">+</label></span
                      >
                    </VisibilitySensor>
                  </div>
                  <div class="text">
                    <h3>연간내원<br />고객수</h3>
                  </div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="wrapper">
                  <div class="value">
                    <VisibilitySensor @change="onChange">
                      <span class="abs"
                        ><span
                          class="tm_counter"
                          data-from="0"
                          data-to="120"
                          data-speed="1200"
                          ><number
                            ref="tm_counter"
                            :to="120"
                            animationPaused
                            :duration="5"
                          /> </span
                        ><label class="small">+</label></span
                      >
                    </VisibilitySensor>
                  </div>
                  <div class="text">
                    <h3>시술콘텐츠</h3>
                  </div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="wrapper">
                  <div class="value">
                    <VisibilitySensor @change="onChange">
                      <span class="abs"
                        ><span class="tm_counter"
                        data-speed="1200"
                          ><number
                            ref="tm_counterclient"
                            :to="500000"
                            animationPaused
                            :duration="5"
                          /> </span
                        ><label class="small">+</label></span
                      >
                    </VisibilitySensor>
                  </div>
                  <div class="text">
                    <h3>Happy<br />Clients</h3>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
      <span class="border moving_effect" data-direction="x"></span>
    </div>
  </div>
</template>

<script>
import VisibilitySensor from "vue-visibility-sensor";
export default {
  name: "Counter",
  components: {
    VisibilitySensor,
  },
  methods: {
    onChange(isVisible) {
      isVisible && this.$refs.tm_counter.restart();
      isVisible && this.$refs.tm_counterk.restart();
      isVisible && this.$refs.tm_counterclient.restart();
    },
  },
};
</script>
