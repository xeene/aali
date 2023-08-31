<template>
  <div class="aali_tm_section" id="contact">
    <div class="aali_tm_contact">
      <div class="container">
        <div class="aali_tm_main_title" data-text-align="center" data-color="dark">
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
                <div class="list_inner" v-html="`<span>Call me</span>
                  <h3>+82-02-6258-3838</h3>` + call"></div>
              </li>
              <li>
                <div class="list_inner" v-html="msg +
                  `<span>Email</span>
                  <h3>
                    <a class='line_anim' href='mailto:shiningmt23@naver.com 
'>shiningmt23@naver.com 
</a></h3>`
                  "></div>
              </li>
            </ul>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <div class="fields">
              <form class="contact_form" id="contact_form" @submit.prevent="submitForm">
                <!-- handSubmit заменила -->
                <div class="returnmessage" data-success="문의는 접수되었습니다! 담당자가 확인 후 연락드리겠습니다."
                  :style="{
                    display: success ? 'block' : 'none',
                  }">
                  <span class="contact_success">
                    Your message has been received, We will contact you soon.
                  </span>
                </div>
                <div class="empty_notice" :style="{ display: error ? 'block' : 'none' }">
                  <span>Please Fill Required Fields</span>
                </div>
                <div class="input_list">
                  <ul>
                    <li>
                      <input id="name" type="text" v-model="name" placeholder="Your Name" />
                    </li>
                    <li>
                      <input id="email" type="text" v-model="email" placeholder="Your Email" />
                    </li>
                    <li>
                      <input id="phone" type="number" placeholder="Your Phone" name="phn" v-model="phone" />
                    </li>
                  </ul>
                </div>
                <div class="message_area">
                  <textarea id="message" placeholder="Your message here" v-model="msge"></textarea>
                </div>
                <div class="aali_tm_button">
                  <a id="send_message" href="#" @click.prevent="submitForm"><span v-html="'Submit Message' + msgSent">
                    
                    </span></a>
                </div>
                 <!-- handSubmit заменила -->

                <!-- If you want change mail address to yours, just open "modal" folder >> contact.php and go to line 4 and change detail to yours.  -->
              </form>
            </div>
          </div>
        </div>
      </div>
      <span class="square moving_effect" data-direction="y" data-reverse="yes"></span>
    </div>
  </div>
</template>

<script>
const WEB3FORMS_ACCESS_KEY = "2011047e-8064-42e8-9298-b0297bcd101b";
//const WEB3FORMS_ACCESS_KEY = "d2040331-5103-4575-ad7e-9331a157b0cb";

import { call, msg, msgSent } from "./svgImage";
export default {
  name: "Contact",
  data() {
    return {
      msgSent,
      call,
      msg,
      // fromData: {
      //   name: "",
      //   email: "",
      //   phone: "",
      //   msg: "",
      // },
        name: "",
        email: "",
        phone: "",
        msge: "",
      error: false,
      success: false,
    };
  },
  methods: {
    handleSubmit() {
      // const { name, email, phone, msg } = this.fromData;
      // if (name && email && phone && msg) {
      //   this.success = true;
      //   setTimeout(() => {
      //     this.success = false;
      //   }, 2000);
      // } else {
      //   this.error = true;
      //   setTimeout(() => {
      //     this.error = false;
      //   }, 2000);
      // }

    },

    async submitForm() {
        const response = await fetch("https://api.web3forms.com/submit", {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Accept: "application/json",
          },
          body: JSON.stringify({
            access_key: WEB3FORMS_ACCESS_KEY,
            name: this.name,
            email: this.email,
            phone: this.phone,
            msge: this.msge,
          }),
        });
        const result = await response.json();
        if (result.success) {
          // console.log(result);
          //alert('문의 접수되었습니다!');
          this.success = true;
        }
      },

  },
};
</script>
