<template>
  <div class="aali_tm_section">
    <div class="aali_tm_copyright">
      <div class="container">
        <div class="copyright_inner">
          <div class="top">
            <div class="logo">
              <img src="img/logo/logo.png" alt="" />
            </div>
            <div class="social">
              <span>Connect</span>
              <ul>
                <li>
                  <a href="http://brand.newstarclinic.co.kr/"><i class = "xi-naver xi-x"></i></a>
                </li>
                <li>
                  <a href="https://www.instagram.com/newstarclinic_official/"><i class="icon-instagram-3"></i></a>
                </li>
                <li>
                  <a href="#"><i class="icon-youtube-2"></i></a>
                </li>
              </ul>
            </div>
          </div>
          <div class="bottom">
            <div class="left">
              <p>
                Designed with love by
                <a
                  class="line_anim"
                  href="https://themeforest.net/user/codeefly"
                  target="_blank"
                  >Codeefly</a
                >
                &copy; {{ new Date().getFullYear() }}
              </p>
            </div>
            <div class="right">
              <ul>
                <li><a class="line_anim" href="#">Terms &amp; Condition</a></li>
                <li><a class="line_anim" href="#">Privacy Policy</a></li>
                <li><a class="line_anim" href="mailto:shiningmt23@naver.com">Support</a></li>
              </ul>
            </div>
          </div>
          <span
            class="border moving_effect"
            data-direction="y"
            data-reverse="yes"
          ></span>
        </div>
      </div>
      <span class="square moving_effect" data-direction="x"></span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>
