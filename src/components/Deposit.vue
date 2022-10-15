<template>
  <!-- mana bu deosit component -->
  <div class="deposit">
    <div class="deposit_wrapper">
      <!-- deposit title -->
      <div class="deposit_title">
        <img class="mx-auto" src="/img/logo.svg" alt="logo.svg" />
        <h1>Пополнение и снятие</h1>
      </div>
      <!-- deposit start -->
      <div class="deposit_in">
        <div class="commission">
          <div class="commission_in">
            <div class="commission_text">
              <h1><span>Наличные</span> без комиссий</h1>
              <p>
                Пополняйте или снимайте наличные по биржевым ценам без комиссий
              </p>
              <a href="">Создать аккаунт сейчас →</a>
            </div>
            <div class="commission_img">
              <img src="/img/dollor_img.png" alt="$_img.png" />
            </div>
          </div>
        </div>
      </div>
      <!-- money -->
      <div class="money">
        <div class="money_in">
          <div class="bank_card">
            <div class="bank_card_in">
              <div class="bank_card_title">
                <h1 class="flex flex-wrap">
                  Банковские <span class="ml-3" style="color: #e20a3e">карты</span>
                </h1>
                <p>Пополнение и вывод от 0% Более 20 банков</p>
              </div>
              <div class="bank_card_img">
                <img src="/img/bank_cards.png" alt="bank_cards.png" />
              </div>
            </div>
          </div>
          <div class="kriptavaluta_code">
            <div class="kriptavaluta">
              <div class="kriptavaluta_in">
                <div class="kriptavaluta_text">
                  <h1>Криптовалюты</h1>
                  <p>Переводите криптовалюту с комиссиями от 1 USDT</p>
                  <h3>USDT, BTC, ETH</h3>
                </div>
                <div class="kriptavaluta_img">
                  <img src="/img/bitcoin_img.png" alt="bitcoin_img.png" />
                </div>
              </div>
            </div>
            <div class="code">
              <div class="code_in">
                <div class="code_text">
                  <div class="code_title">
                    <img src="/img/card_blue.svg" alt="card_blue.svg" />
                    <h1>Code</h1>
                  </div>
                  <p>
                    Переводите любые активы между пользователями биржи без
                    комиссий
                  </p>
                </div>
                <div class="code_img">
                  <img src="/img/blue_card_img.png" alt="blue_card_img.png" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- valuta -->
    </div>
  </div>
</template>

<script>
export default {
  name: "Deposit",
};
</script>

<style scoped>
/* deposit start---------------------------------------- */
.deposit_wrapper {
  max-width: 1920px;
  padding: 0 30px;
  margin: 0 auto;
}
.deposit_in {
  max-width: 1700px;
  margin: 0 auto;
}
/* deposit title */
.deposit_title {
  text-align: center;
  margin-bottom: 60px;
}
.deposit_title h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  text-align: center;
}
.deposit_in {
  border-radius: 40px;
  background-color: #fff;
}
/* commission */
.commission {
  margin-bottom: 20px;
}
.commission_in {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
}
.commission_text {
  padding: 50px 0px 50px 100px;
}
.commission_text h1 {
  max-width: 760px;
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  letter-spacing: -0.02em;
  color: #000;
  margin-bottom: 25px;
}
.commission_text h1 span {
  background: linear-gradient(100.08deg, #3b8e26 20.28%, #78cf62 58.66%),
    linear-gradient(0deg, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #1f850e;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.commission_text p {
  margin-bottom: 40px;
  max-width: 671px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 34px;
  line-height: 141.02%;
  color: #1e1f28;
}
.commission_text a {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 34px;
  line-height: 149%;
  color: #000000;
}
.commission_img img {
  padding: 0px 100px 0px 0px;
}
/* money */
.money_in {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  max-width: 1700px;
  margin: 0 auto;
}
.bank_card {
  border-radius: 40px;
  background-color: #fff;
  width: 850px;
  overflow: hidden;
}
.bank_card_title {
  padding: 50px 0px 0px 50px;
}
.bank_card_title h1 {
  white-space: nowrap;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  letter-spacing: -0.02em;
  color: #000000;
  margin-bottom: 20px;
}
.bank_card_title p {
  max-width: 527px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 135.19%;
  color: #000000;
  margin-bottom: 30px;
}
.bank_card_img img {
  position: relative;
  width: 800px;
  right: -28px;
  bottom: -5px;
}

/* kriptavaluta_code */
.kriptavaluta_code {
  margin-left: 25px;
}
.kriptavaluta {
  margin-bottom: 25px;
  width: 850px;
  background-color: #fff;
  background: linear-gradient(
      0deg,
      rgba(255, 255, 255, 0.64),
      rgba(255, 255, 255, 0.64)
    ),
    linear-gradient(0deg, #ebeff0, #ebeff0), #191e25;
  border-radius: 39px;
  overflow: hidden;
}
.kriptavaluta_in {
  display: flex;
  align-items: stretch;
  justify-content: space-between;
}
.kriptavaluta_text {
  position: relative;
  z-index: 4;
  padding: 65px 0px 65px 65px;
}
.kriptavaluta .kriptavaluta_in .kriptavaluta_text h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  letter-spacing: -0.02em;
  color: #1e1f28;
  margin-bottom: 32px;
}
.kriptavaluta_in .kriptavaluta_text p {
  max-width: 591px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 135.19%;
  color: #1e1f28;
  margin-bottom: 60px;
}
.kriptavaluta_in .kriptavaluta_text h3 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 36px;
  line-height: 49px;
  letter-spacing: -0.02em;
  color: #1e1f28;
  margin-bottom: 15px;
}
.kriptavaluta_img {
  display: flex;
  align-items: stretch;
}
.kriptavaluta_img img {
  position: relative;
  z-index: 1;
}
.code {
  width: 850px;
  overflow: hidden;
  background: linear-gradient(0deg, #226fff, #226fff), #ffffff;
  border-radius: 39px;
}
.code_in {
  display: flex;
  align-items: stretch;
  justify-content: space-between;
}
.code_title {
  display: flex;
  align-items: center;
  margin-bottom: 45px;
}
.code_title h1 {
  margin-left: 20px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 86px;
  text-align: right;
  letter-spacing: -0.02em;
  color: #ffffff;
}
.code_text {
  padding: 65px 0px 65px 65px;
}
.code_text p {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 49px;
  color: #ffffff;
}
.code_img img {
  display: flex;
  align-items: stretch;
}
</style>