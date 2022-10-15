<template>
  <div>
    <footer>
    <div class="foter-in">
      <div class="grid grid-cols-4 items-center footer-top">
        <div class="col-span-4 sm:col-span-2">
          <img src="/img/logo.svg" alt="" />
          <p>Криптофиатная биржа</p>
        </div>
        <div class="col-span-4 sm:col-span-2 footer-messengers flex sm:justify-end">
          <a href="#"><img src="/img/telegram.svg" alt="" /></a>
          <a href="#"><img src="/img/twitter.svg" alt="" /></a>
          <a href="#"><img src="/img/wkontact.svg" alt="" /></a>
          <a href="#"><img src="/img/vc.svg" alt="" /></a>
        </div>
      </div>

      <div class="footer-bottom">
        <div class="grid grid-cols-9">
          <div class="col-span-9 md:col-span-4 lg:col-span-3">
            <ul>
              <li>ИНФОРМАЦИЯ</li>
              <li><a href="#">Комиссии и лимиты</a></li>
              <li><a href="#">Rapira Code</a></li>
              <li><a href="#">Торги</a></li>
            </ul>
          </div>
          <div class="col-span-9 md:col-span-4 lg:col-span-3">
            <ul>
              <li>Документы</li>
              <li><a href="#">Правила и комиссии</a></li>
              <li><a href="#">Политика конфиденциальности</a></li>
              <li><a href="#">Пользовательское соглашение</a></li>
              <li><a href="#">Политика Cookie</a></li>
            </ul>
          </div>
          <div class="col-span-9 md:col-span-9 lg:col-span-3">
            <ul>
              <li>ПОДДЕРЖКА</li>
              <li>
                Общие вопросы support@rapira.net @rapirabot 
              </li>
              <li>AML, KYC, официальные запросы compliance@rapira.net</li>
              <li>Юридические вопросы legal@rapira.net</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
  <div class="empty-space">

      </div>
  </div>
</template>


<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
footer {
  max-width: 1920px;
  margin: 0 auto;
  padding: 0 30px;
}
.foter-in {
  max-width: 1700px;
  margin: 0 auto;
}
.footer-top p {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 38px;
  color: #000000;
}
.footer-messengers img {
  width: 55px;
  height: 55px;
  margin-left: 35px;
}
.footer-bottom {
  padding: 86px 0 130px;
}
.footer-bottom ul li:first-child {
  font-family: "Inter";
  font-style: normal;
  font-weight: 700;
  font-size: 28px;
  line-height: 125%;
  color: #3c4550;
  margin-bottom: 31px;
}
.footer-bottom ul li{
  font-family: "Inter";
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 125%;
  color: #3c4550;
  margin-bottom: 14px;
  display: block;
}
.footer-bottom ul li a {
  font-family: "Inter";
  font-style: normal;
  font-weight: 400;
  font-size: 28px;
  line-height: 125%;
  color: #3c4550;
  margin-bottom: 14px;
  display: block;
}
.footer-bottom ul li a:hover {
  text-decoration-line: underline;
}
.empty-space{
height: 121px;
border-top: 1px solid rgba(0, 0, 0, 0.22);
}
</style>