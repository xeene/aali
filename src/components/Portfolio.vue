<template>
  <div class="aali_tm_section help" id="portfolio">
    <div class="aali_tm_portfolio wow fadeInUp" data-wow-duration="1s">
      <div class="container">
        <div class="aali_tm_main_title" data-text-align="center" data-color="light">
          <span>Selected works</span>
          <h3>Check Our purpose </h3>
        </div>
        <div class="portfolio_filter">
          <ul>
            <li><a href="#" class="current" data-filter="*">All</a></li>

            <!-- <li><a href="#" data-filter=".vimeo">Vimeo</a></li>
            <li><a href="#" data-filter=".youtube">Youtube</a></li>
            <li><a href="#" data-filter=".soundcloud">Soundcloud</a></li> -->

            <li><a href="#" data-filter=".network">Network</a></li>
            <!-- Netwok -->
            <li><a href="#" data-filter=".beauty">Beauty</a></li>
            <!-- Beauty -->
            <li><a href="#" data-filter=".global">Global</a></li>
            <!-- Global -->
          </ul>
        </div>
        <div class="portfolio_list">
          <ul class="gallery_zoom">
            <!-- <li class="vimeo gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/thumbs/1-1.jpg" alt="" />
                  <div class="main" data-img-url="img/portfolio/1.jpg"></div>
                </div>
                <div class="overlay"></div>
                <div v-html="vimeo"></div>
                <div class="details">
                  <span>Vimeo</span>
                  <h3>New Laptop</h3>
                </div>
                <a
                  class="aali_tm_full_link popup-vimeo"
                  href="#"
                  @click.prevent="() => onClick('vimeo', '337293658')"
                ></a>
              </div>
            </li>
            <li class="youtube gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/thumbs/1-1.jpg" alt="" />
                  <div class="main" data-img-url="img/portfolio/2.jpg"></div>
                </div>
                <div class="overlay"></div>
                <div v-html="youtube"></div>
                <div class="details">
                  <span>Youtube</span>
                  <h3>Best Phone</h3>
                </div>
                <a
                  class="aali_tm_full_link popup-youtube"
                  href="#"
                  @click.prevent="() => onClick('youtube', '7e90gBu4pas')"
                ></a>
              </div>
            </li>
            <li class="soundcloud gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/thumbs/1-1.jpg" alt="" />
                  <div class="main" data-img-url="img/portfolio/3.jpg"></div>
                </div>
                <div class="overlay"></div>
                <div v-html="soundcloud"></div>
                <div class="details">
                  <span>Soundcloud</span>
                  <h3>Smart Headphone</h3>
                </div>
                <a
                  class="aali_tm_full_link soundcloude_link mfp-iframe audio"
                  href="#"
                  @click.prevent="() => onClick('soundcloud', '471954807')"
                ></a>
              </div>
            </li> -->
            <li class="network gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/portfolio/4.png" alt="" />
                  <div class="main" data-img-url="img/portfolio/4.png"></div>
                </div>
                <div class="overlay"></div>
                <!-- <div v-html="text"></div> -->
                <div class="details">
                  <!-- <span>Detail</span> -->
                  <h3>EXPENSION OF DOMESTIC HOSPITAL BRANCHES
                  </h3>
                </div>
                <a class="aali_tm_full_link portfolio_popup" href="#" @click.prevent="active = 1"></a>
                <!-- поп-ап -->
                <div :class="`${active === 1 ? '' : 'hidden_content'}`">
                  <ModalBox :close="close">
                    <div class="popup_details">
                      <div class="top_image">
                        <img src="img/portfolio/popup_1.jpg" alt="" />
                        <div class="main" data-img-url="img/portfolio/popup_1.jpg"
                          style="background-image: url('img/portfolio/popup_1.jpg')"></div>
                        <!-- ^data-img-url - изображение внутри попапа -->
                      </div>

                    </div>
                  </ModalBox>
                </div>
              </div>
            </li>

            <li class="beauty gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/portfolio/5.png" alt="" />
                  <!-- ^img нужен, чтобы задать размер прекью-коробке -->
                  <div class="main" data-img-url="img/portfolio/5.png"></div>
                  <!-- ^само изображение превью-коробки -->
                </div>
                <div class="overlay"></div>
                <!-- <div v-html="maximize"></div> -->
                <div class="details">
                  <!-- <span>Image</span> -->
                  <h3>DEVELOPMENT OF BEAUTY PRODUCTS
                  </h3>
                </div>
                <!-- <a
                  class="aali_tm_full_link zoom"
                  href="#"
                  @click.prevent="() => onClick('img', 'img/portfolio/5.jpg')"
                ></a> -->
                <a class="aali_tm_full_link portfolio_popup" href="#" @click.prevent="active = 3"></a>
                <!-- поп-ап -->
                <div :class="`${active === 3 ? '' : 'hidden_content'}`">
                  <ModalBox :close="close">
                    <div class="popup_details">
                      <div class="top_image">
                        <img src="img/portfolio/popup_2.jpg" alt="" />
                        <div class="main" data-img-url="img/portfolio/popup_2.jpg"
                          style="background-image: url('img/portfolio/popup_2.jpg')"></div>
                      </div>
                      <div class="portfolio_main_title">
                        <!-- <span>Detail</span> 
                        <h3>GLOBALIZATION OF NETWORK & BEAUTY PRODUCTS</h3>
                        <div></div>-->
                      </div>

                    </div>
                  </ModalBox>
                </div>
              </div>
            </li>

            <li class="global gallery_item">
              <div class="list_inner">
                <div class="image">
                  <img src="img/portfolio/6.png" alt="" />
                  <div class="main" data-img-url="img/portfolio/6.png"></div>
                </div>
                <div class="overlay"></div>
                <!-- <div v-html="text"></div> -->
                <div class="details">
                  <!-- <span>Detail</span> -->
                  <h3>GLOBALIZATION OF NETWORK & BEAUTY PRODUCTS
                  </h3>
                </div>
                <a class="aali_tm_full_link portfolio_popup" href="#" @click.prevent="active = 2"></a>
                <!-- поп-ап -->
                <div :class="`${active === 2 ? '' : 'hidden_content'}`">
                  <ModalBox :close="close">
                    <div class="popup_details">
                      <div class="top_image">
                        <img src="img/portfolio/popup_3.jpg" alt="" />
                        <div class="main" data-img-url="img/portfolio/popup_3.jpg"
                          style="background-image: url('img/portfolio/popup_2.jpg')"></div>
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
    <MagnificPopUp :modal="modal" :close="closeModal" :name="name" :src="src" />
  </div>
</template>

<script>
import MagnificPopUp from "./MagnificPopUp.vue";
import ModalBox from "./ModalBox.vue";
import { maximize, soundcloud, text, vimeo, youtube } from "./svgImage";
export default {
  name: "Portfolio",
  data() {
    return {
      vimeo,
      youtube,
      soundcloud,
      text,
      maximize,
      // props
      name: "",
      src: "",
      modal: false,
      // Content
      active: 0,
    };
  },
  mounted() {
    let Isotope = require("isotope-layout");
    setTimeout(() => {
      let iso = new Isotope(".gallery_zoom", {
        itemSelector: ".gallery_item",
        layoutMode: "fitRows",
      });
      let filterFns = {
        // show if number is greater than 50
        numberGreaterThan50: function (itemElem) {
          let number = itemElem.querySelector(".number").textContent;
          return parseInt(number, 10) > 50;
        },
        // show if name ends with -ium
        ium: function (itemElem) {
          let name = itemElem.querySelector(".name").textContent;
          return name.match(/ium$/);
        },
      };
      // bind filter button click filter main funtion
      let filtersElem = document.querySelector(".portfolio_filter ul");
      filtersElem.addEventListener("click", function (event) {
        if (event.target.getAttribute("data-filter")) {
          let filterValue = event.target.getAttribute("data-filter");
          filterValue = filterFns[filterValue] || filterValue;
          iso.arrange({ filter: filterValue });
        }
      });
    }, 1000);
  },
  methods: {
    onClick(name, src) {
      this.name = name;
      this.src = src;
      this.modal = true;
    },
    closeModal() {
      this.modal = false;
      this.name = "";
      this.src = "";
    },
    close() {
      this.active = 0;
    },
  },
  components: { MagnificPopUp, ModalBox },
};
</script>
