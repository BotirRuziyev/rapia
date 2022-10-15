<template>
  <div>
    <div class="mx-auto money-big-wrapper">
      <img class="block mx-auto" src="/img/logo.svg" />
      <h1 class="block zadacha">Заточена на деньги</h1>
      <div class="money-wrapper block mx-auto">
        <div class="money">
          <div class="money-item">
            <img src="/img/money_text.svg" class="money_text_img" />
          </div>
          <div class="money-item"><img src="/img/img_foiz.png" /></div>
        </div>
      </div>
      <div class="money-bottom-wrapper block mx-auto">
        <div class="money-bottom">
          <div class="money-text">
            <h1>Надёжно храним вашу криптовалюту</h1>
            <p>Надежность блокчейна в полной интеграции с Рапира.</p>
            <a href="#">Создать кошелек сейчас →</a>
          </div>
          <div class="galochka_card">
            <img src="/img/galchka_green_icon.svg" />
            <p>Более 90% активов хранятся на холодных хранилищах</p>
          </div>
          <div class="money-img">
            <img src="/img/galchka_img.png" />
          </div>
        </div>
      </div>
    </div>
    <!-- counter up start -->
    <div class="count_money_wrapper">
      <div class="count_money_in">
        <div>
          <h1>
            $<ICountUp
              :delay="delay"
              :endVal="endVal1"
              :options="options"
              @ready="onReady"
            />
          </h1>
          <p>Oбьем торгов за 7 день</p>
        </div>
        <div>
          <h1>
            $<ICountUp
              :delay="delay"
              :endVal="endVal2"
              :options="options"
              @ready="onReady2"
            />
          </h1>
          <p>Oбьем торгов за день</p>
        </div>
        <div>
          <h1>
            <ICountUp
              :delay="delay"
              :endVal="endVal3"
              :options="options"
              @ready="onReady3"
            />
          </h1>
          <p>активных трейдеров</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ICountUp from "vue-countup-v2";
export default {
  components: {
    ICountUp,
  },
  data() {
    return {
      delay: 1000,
      endVal1: 7764002,
      endVal2: 921545,
      endVal3: 36286,
      options: {
        useEasing: true,
        useGrouping: true,
        separator: " ",
        decimal: " ",
        prefix: "",
        suffix: "",
      },
    };
  },
  methods: {
    onReady: function (instance, CountUp) {
      const that = this;
      instance.update(that.endVal1);
    },
    onReady2: function (instance, CountUp) {
      const that = this;
      instance.update(that.endVal2);
    },
    onReady3: function (instance, CountUp) {
      const that = this;
      instance.update(that.endVal3);
    },
  },
};
</script>

<style scoped>
.money-big-wrapper {
  max-width: 1920px;
  margin-top: 150px;
  padding: 0 30px;
}
.zadacha {
  text-align: center;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  margin-bottom: 72px;
  margin-top: 5px;
}
.money-wrapper {
  max-width: 1700px;
  margin: 0 auto;
  display: block;
  background: #ffffff;
  box-shadow: 0px 4px 86px rgba(16, 36, 66, 0.1);
  border-radius: 36px;
  max-height: 329px;
  margin-bottom: 25px;
}
.money {
  display: flex;
  height: 100%;
  justify-content: space-around;
  align-items: center;
}

.money-item img {
  max-width: 450px;
}
.money-bottom-wrapper {
  max-width: 1700px;
}
.money-bottom {
  padding: 70px 87px;
  position: relative;
  display: flex;
  margin: 0 auto;
  box-sizing: border-box;
  height: 649px;
  background: linear-gradient(0deg, #fafbfb, #fafbfb), #ffffff;
  box-shadow: 0px 4px 86px rgba(16, 36, 66, 0.1);
  border-radius: 41px;
  justify-content: space-around;
  align-items: center;
}
.money-img img {
  width: 707px;
  height: 617px;
}
.galochka_card {
  display: flex;
  position: absolute;
  bottom: 46px;
  right: 10%;
  background: rgba(255, 255, 255, 0.85);
  box-shadow: 0px -2px 45px rgba(0, 0, 0, 0.07);
  backdrop-filter: blur(6px);
  border-radius: 26px;
  flex-wrap: nowrap;
  max-width: 607px;
  max-height: 127px;
  padding: 22px 25px;
  justify-content: space-around;
  align-items: center;
}
.galochka_card p {
  font-family: "Roboto", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 32px;
  line-height: 131.5%;
  color: #697582;
  max-width: 486px;
  padding-left: 25px;
  padding-right: 15px;
}
.galchka_card img {
  width: 63px;
  height: 90px;
}
.money-bottom .money-text h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 72px;
  line-height: 117%;
  letter-spacing: 0.02em;
  color: #000000;
  margin-bottom: 45px;
}
.money-bottom .money-text p {
  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 40px;
  line-height: 149%;
  letter-spacing: 0.02em;
  color: #000000;
  margin-bottom: 105px;
}
.money-bottom .money-text a {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 149%;
  color: #000000;
}
.count_money_wrapper {
  margin-top: 120px;
  width: 100%;
  padding: 18px 0;
  background: #1e2022;
}
.count_money_wrapper .count_money_in {
  width: 100%;
  max-width: 1700px;
  padding: auto 0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: 0 auto;
  background-image: url('/public/img/bg_dollor.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  padding: 18px 0;
}

.count_money_wrapper .count_money_in div h1 {
  color: #fff;
  font-size: 65px;
  font-weight: 700;
}

.count_money_wrapper .count_money_in div p {
  color: #fff;
  opacity: 0.5;
  text-align: center;
  font-size: 22px;
}

@media (max-width: 1600px) {
  .money-big-wrapper {
    margin-top: 100px;
  }
  .money-item .money_text_img {
    max-width: 360px;
    padding-left: 40px;
  }
  .money-bottom {
    height: 500px;
  }
  .money-bottom .money-text h1 {
    font-size: 54px;
    max-width: 844px;
  }
  .money-img img {
    width: 507px;
    height: 417px;
  }
  .galochka_card {
    max-width: 457px;
    bottom: 5%;
  }
  .galochka_card p {
    font-size: 22px;
  }
  .money-bottom .money-text a {
    font-size: 30px;
  }
  .money-bottom .money-text p {
    margin-bottom: 60px !important;
  }
}
</style>
