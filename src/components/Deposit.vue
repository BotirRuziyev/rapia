<template>
  <div class="deposit_wrapper">
    <div class="deposit_title">
      <div class="deposit_title_logo">
        <img src="/img/logo.svg" alt="deposit_logo.svg" />
      </div>
      <h1>Пополнение и снятие</h1>
    </div>
    <div class="deposit_in">
      <div class="deposit_cash">
        <div class="deposit_cash_text">
          <h1><span style="color: #1f850e">Наличные</span> без комиссий</h1>
          <p>Пополняйте или снимайте наличные по биржевым ценам без комиссий</p>
          <a href="">Создать аккаунт сейчас →</a>
        </div>
        <div class="deposit_img">
          <img src="/img/dollor_img.png" alt="dollor_img.png" />
        </div>
      </div>
    </div>
    <div class="deposit_currency">
      <div class="deposit_currency_in">
        <div class="deposit_currency_bank_card">
          <h1>Банковские <span style="color: #e20a3e">карты</span></h1>
          <p>Пополнение и вывод от 0% Более 20 банков</p>
          <div><img src="/img/bank_cards.png" alt="bank_cards.png" /></div>
        </div>
        <div class="deposit_currency_bitcoin">
          <div class="currency">
            <div class="currency_text">
              <h1>Криптовалюты</h1>
              <p>Переводите криптовалюту с комиссиями от 1 USDT</p>
              <h3>USDT, BTC, ETH</h3>
            </div>
            <div class="currency_img">
              <img src="/img/bitcoin_img.png" alt="bitcoin_img.png" />
            </div>
          </div>
          <div class="code">
            <div class="code_text">
              <div class="code_title">
                <img src="/img/card_logo.png" alt="card_logo.png" />
                <h1>Code</h1>
              </div>
              <p>
                Переводите любые активы между пользователями биржи без комиссий
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
</template>

<script>
export default {
  name: "Deposit",
};
</script>

<style scoped>
.deposit_wrapper {
  max-width: 1920px;
  margin: 0 auto;
  padding: 0 30px;
}
.deposit_in {
  max-width: 1700px;
  margin: 0 auto;
  
}
.deposit_title h1 {
  margin-top: 5px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  text-align: center;
  margin-bottom: 60px;
}
.deposit_title_logo {
  display: flex;
  align-items: center;
  justify-content: center;
}
.deposit_in {
  background: #ffffff;
  box-shadow: 0px 4px 70px rgba(24, 105, 23, 0.07);
  border-radius: 58px;
}
.deposit_cash {
  display: flex;
  align-content: flex-start;
  justify-content: space-between;
  margin-bottom: 25px;
}
.deposit_cash_text {
  max-width: 770px;
  padding: 50px 0px 50px 50px;
}
.deposit_img img {
  padding-top: 20px;
  padding-bottom: 20px;
  padding-right: 50px;
}
.deposit_cash h1 span {
  margin-right: 15px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  display: flex;
  align-items: center;
  letter-spacing: -0.02em;
  background: linear-gradient(100.08deg, #3b8e26 20.28%, #78cf62 58.66%),
    linear-gradient(0deg, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #1f850e;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.deposit_cash h1 {
  white-space: nowrap;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}
.deposit_cash p {
  margin-bottom: 40px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 34px;
  line-height: 141.02%;
  color: #1e1f28;
}
.deposit_cash a {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 34px;
  line-height: 149%;
  color: #000000;
}
/* --------- */
.deposit_currency {
  max-width: 1920px;
  margin: 0 auto;
}
.deposit_currency_in {
  max-width: 1700px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.deposit_currency_bitcoin {
  flex: 1;
}
.deposit_currency_bank_card {
  flex: 1;
  margin-right: 25px;
  padding: 50px 0px 0px 50px;
  background: linear-gradient(0deg, #ffffff, #ffffff), #fff4f9;
  border-radius: 39px;
}
.deposit_currency_bank_card h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  letter-spacing: -0.02em;
  color: #000000;
  margin-bottom: 24px;
  max-width: 567px;
}
.deposit_currency_bank_card p {
  max-width: 500px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 135.19%;
  color: #000000;
  margin-bottom: 40px;
}
/* criptavaluta */
.currency {
  flex: 1;
  overflow: hidden;
  background-color: #fff;
  border-radius: 39px;
  display: flex;
  margin-bottom: 25px;
  position: relative;
  
}
.currency_text {
  padding: 52px;
  position: relative;
  z-index: 2;
}
.currency_img {
  max-width: 265px;
  position: absolute;
  right: 0;
  height: 100%;
}
.currency_img img {
  height: 100%;
}
.currency_text h1 {
  margin-bottom: 32px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 82px;
  letter-spacing: -0.02em;
  color: #1e1f28;
}
.currency_text p {
  margin-bottom: 60px;
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 135.19%;
  color: #1e1f28;
}
.currency_text h3 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 36px;
  line-height: 49px;
  letter-spacing: -0.02em;
  color: #1e1f28;
}
.code {
  overflow: hidden;
  height: 432px;
  background: linear-gradient(0deg, #226fff, #226fff), #ffffff;
  border-radius: 39px;
  display: flex;
  align-content: flex-start;
  justify-content: space-between;
}
.code_title {
  display: flex;
  align-items: center;
  margin-bottom: 40px;
}
.code_text {
  flex: 2;
  padding: 70px 0px 0px 50px;
}
.code_img {
  flex: 1;
}
.code_img img {
  object-fit: contain;
}
.code_text h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 63px;
  line-height: 86px;
  text-align: right;
  letter-spacing: -0.02em;
  color: #ffffff;
  white-space: nowrap;
}
.code_text p {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 36px;
  line-height: 49px;
  color: #ffffff;
}
</style>