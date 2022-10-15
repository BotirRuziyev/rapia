<template>
  <div class="home flex flex-col justify-center items-center">
    <div class="home-header">
      <div class="title">Биржевой обмен</div>
      <div class="description">
        Гарантия лучшей цены без посредников <br />
        на криптофиатной бирже Рапира
      </div>
    </div>
    <div class="rubles-to-dollars flex">
      <div class="give">
        <p>Отдаю</p>
        <div class="select-kours">
          <div @click="optionActive" class="dollor flex items-center">
            <img src="/img/dollor-icon.svg" alt="" /><span class="dollor_sum"
              >1000</span
            >
            USDT
            <img
              class="ml-4 uploads-icon"
              src="/img/lang-select-icon.svg"
              alt=""
            />
          </div> 
          <div class="option-content">
            <div class="option" @click="count(100)"><span>100</span> USDT</div>
            <div class="option" @click="count(1000)">
              <span>1000</span> USDT
            </div>
            <div class="option" @click="count(10000)">
              <span>10000</span> USDT
            </div>
          </div>
        </div>
        <p>1 USDT ≈ 63.15 RUB</p>
      </div>
      <img class="exchange" src="/img/exchange.svg" alt="" />
      <div class="receive">
        <p>Получаю ≈</p>
        <div class="select-kours">
          <div class="dollor flex items-center">
            <img src="/img/rubl_icon.svg" alt="" /><span
              class="rubl_sum"
            ></span>
            RUB
            <img class="ml-4" src="/img/lang-select-icon.svg" alt="" />
          </div>
        </div>
      </div>
      <div class="flex items-center">
        <a href="#">ОБМЕНЯТЬ</a>
      </div>
    </div>
    <img class="home-red-img" src="/img/home-red.svg" alt="">
    <img class="home-blue-img" src="/img/home-blue.svg" alt="">
  </div>
</template>

<script>
import { onMounted } from "vue";
export default {
  name: "Home",

  methods: {
    count(sum) {
      let rubl_sum = document.querySelector(".rubl_sum");
      let dollor_sum = document.querySelector(".dollor_sum");
      let option_content = document.querySelector(".option-content");
      let uploads_icon = document.querySelector(".uploads-icon");
      rubl_sum.innerHTML = sum * 63.15;
      dollor_sum.innerHTML = sum;
      option_content.classList.remove("option-content-active");
      uploads_icon.classList.remove("uploads_icon_active");
    },
    optionActive() {
      let option_content = document.querySelector(".option-content");
      let uploads_icon = document.querySelector(".uploads-icon");
      option_content.classList.add("option-content-active");
      uploads_icon.classList.add("uploads_icon_active");
    },
  },
  mounted() {
    let rubl_sum = document.querySelector(".rubl_sum");
    let dollor_sum = document.querySelector(".dollor_sum");

    rubl_sum.innerHTML = Number(dollor_sum.textContent) * 63.15;
  },
};
</script>

<style scoped>
.home {
  max-width: 1920px;
  margin: 0 auto;
  position: relative;
  padding: 80px 0 120px;
}
.home-header {
  margin-bottom: 72px;
  position: relative;
  z-index: 2;
}
.home-header .title {
  margin-bottom: 24px;
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 82px;
  line-height: 113%;
  text-align: center;
  color: #07080a;
}
.home-header .description {
  margin-bottom: 24px;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 141.02%;
  text-align: center;
  color: #434343;
}
.rubles-to-dollars {
  background: #ffffff30;
  backdrop-filter: blur(15.5px);
  border-radius: 19px;
  padding: 43px 47px;
  position: relative;
  z-index: 1;
}
.select-kours {
  background: #ffffff;
  border-radius: 49px;
  padding: 10px 15px;
  margin: 7px 0;
  position: relative;
}
.dollor {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 141.02%;
  text-align: right;
  color: #000000;
  pointer-events: auto;
  cursor: pointer;
}
.option-content {
  width: 100%;
  position: absolute;
  top: 110%;
  left: 0;
  background-color: #fefefe;
  border-radius: 20px;
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 141.02%;
  color: #000000;
  pointer-events: auto;
  cursor: pointer;
  padding: 20px 0;
  opacity: 0;
  transition: 0.5s;
  display: none;
  max-height: 300px;
  overflow-y: auto;
}
.uploads-icon {
  transition: 0.5s;
}
.uploads_icon_active {
  transform: rotate(-180deg);
}
.option-content-active {
  display: block;
  opacity: 1;
}
.option {
  padding: 10px 20px;
}
.option:hover {
  background-color: #f5f5f5;
}
.dollor span {
  margin: 0 11px 0 65px;
}
.rubles-to-dollars p {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  display: flex;
  align-items: center;
  letter-spacing: -0.02em;
  color: #8392a9;
}
.rubles-to-dollars a {
  display: block;
  background: linear-gradient(0deg, #005ff9, #005ff9), #ffffff;
  border-radius: 76px;
  padding: 14px 25px;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 700;
  font-size: 28px;
  line-height: 141.02%;
  text-align: center;
  letter-spacing: 0.025em;
  color: #fff;
  margin-left: 40px;
}
.exchange {
  margin: 0 31px;
}
.home-red-img{
  position: absolute;
  right: 0;
  top: -18%;
}
.home-blue-img{
  position: absolute;
  top: 10%;
  left: 0;
}
</style>