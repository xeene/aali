<template>
  <div class="aali_tm_section">
    <div class="aali_tm_copyright">
      <div class="container">
        <div class="copyright_inner">
          <div class="top">
            <div class="logo">
              <img src="img/logo/dk_2.png" alt="" />
            </div>
            <div class = "right_top">
              <div  class="social"><span>Connect</span>
              <ul>
                <li>
                  <a href="http://brand.newstarclinic.co.kr/"><img src="img/logo/ns.svg" class = "ns_logo"></a>
                </li>
                <li>
                  <a href="https://www.instagram.com/newstarclinic_official/"><i class="icon-instagram-3"></i></a>
                </li>
                <li>
                  <a href="#"><i class="icon-youtube-2"></i></a>
                </li>
              </ul></div>
              <div class = "address">
                <ul>
                  <li>서울특별시 서초구 강남대로69길 8, 10층 1018호 (서초동, 케이아이타워 (KI타워))</li>
                  <li>대표: 장수정 | 사업자번호 : 461-81-03045</li>
                  <li>T. +82-02-6258-3838 | M. +82-010-5094-5423</li>
                  <li>E-mail: shiningmt23@naver.com</li>
                </ul>
              </div>
              
            </div>
          </div>
          <div class="bottom">
            <div class="left">
              <p>
COPYRIGHT
                &copy; {{ new Date().getFullYear() }}
                (주)미산 ALL RIGHT RESERVED
              </p>
            </div>
            <div class="right">
              <ul>
                <li><a class="line_anim" href="http://newstarclinic.co.kr/page/?pid=provision">회원이용약관</a></li>
                <li><a class="line_anim" href="http://newstarclinic.co.kr/page/?pid=privacy">개인정보처리방침
</a></li>
                <li><a class="line_anim" href="http://newstarclinic.co.kr/page/?pid=noemail">이메일무단수집거부</a></li>
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
