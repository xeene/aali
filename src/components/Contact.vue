<template>
  <div class="aali_tm_section" id="contact">
    <div class="aali_tm_contact">
      <div class="container">
        <div
          class="aali_tm_main_title"
          data-text-align="center"
          data-color="dark"
        >
          <span>Get in Touch</span>
          <h3>Connect with Us with Confidence</h3>
        </div>
        <div class="contact_inner">
          <div class="left wow fadeInLeft" data-wow-duration="1s">
            <div class="text">
              <p>
                뉴스타 클리닉 가맹점 모집 및 미산 제품 문의

              </p>
            </div>
            <ul>
              <li>
                <div
                  class="list_inner"
                  v-html="
                    `<span>Call me</span>
                  <h3>+82-00-000-0000</h3>` + call"></div>
              </li>
              <li>
                <div
                  class="list_inner"
                  v-html="
                    msg +
                    `<span>Email</span>
                  <h3>
                    <a class='line_anim' href='mailto:shiningmt23@naver.com 
'>shiningmt23@naver.com 
</a></h3>`
                  "
                ></div>
              </li>
            </ul>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <div class="fields">
              <form
                class="contact_form"
                id="contact_form"
                @submit.prevent="handleSubmit"
              >
                <div
                  class="returnmessage"
                  data-success="Your message has been received, We will contact you soon."
                  :style="{
                    display: success ? 'block' : 'none',
                  }"
                >
                  <span class="contact_success">
                    Your message has been received, We will contact you soon.
                  </span>
                </div>
                <div
                  class="empty_notice"
                  :style="{ display: error ? 'block' : 'none' }"
                >
                  <span>Please Fill Required Fields</span>
                </div>
                <div class="input_list">
                  <ul>
                    <li>
                      <input
                        id="name"
                        type="text"
                        v-model="fromData.name"
                        placeholder="Your Name"
                      />
                    </li>
                    <li>
                      <input
                        id="email"
                        type="text"
                        v-model="fromData.email"
                        placeholder="Your Email"
                      />
                    </li>
                    <li>
                      <input
                        id="phone"
                        type="number"
                        placeholder="Your Phone"
                        name="phn"
                        v-model="fromData.phone"
                      />
                    </li>
                  </ul>
                </div>
                <div class="message_area">
                  <textarea
                    id="message"
                    placeholder="Your message here"
                    v-model="fromData.msg"
                  ></textarea>
                </div>
                <div class="aali_tm_button">
                  <a id="send_message" href="#" @click.prevent="handleSubmit"
                    ><span v-html="'Submit Message' + msgSent"> </span
                  ></a>
                </div>

                <!-- If you want change mail address to yours, just open "modal" folder >> contact.php and go to line 4 and change detail to yours.  -->
              </form>
            </div>
          </div>
        </div>
      </div>
      <span
        class="square moving_effect"
        data-direction="y"
        data-reverse="yes"
      ></span>
    </div>
  </div>
</template>

<script>
import { call, msg, msgSent } from "./svgImage";
export default {
  name: "Contact",
  data() {
    return {
      msgSent,
      call,
      msg,
      fromData: {
        name: "",
        email: "",
        phone: "",
        msg: "",
      },
      error: false,
      success: false,
    };
  },
  methods: {
    handleSubmit() {
      const { name, email, phone, msg } = this.fromData;
      if (name && email && phone && msg) {
        this.success = true;
        setTimeout(() => {
          this.success = false;
        }, 2000);
      } else {
        this.error = true;
        setTimeout(() => {
          this.error = false;
        }, 2000);
      }
    },
  },
};
</script>
