<template>
  <div id="contact" class="mx-auto">
    <h1 class="text-center">Начните сейчас</h1>
    <p class="text-center">Быстрая регистрация за 1 минуту</p>
    <router-link class="block text-center mx-auto registration" to="#"
      >Зарегистрироваться</router-link
    >
    <div class="contact_in mx-auto">
      <div class="contact_in_left">
        <h5>Круглосуточная поддержка</h5>
        <p>
          Наша поддержка на связи 24/7 в режиме реального времени всегда готова
          помочь
        </p>
      </div>
      <div class="contact_in_right">
        <img src="/img/money_telegram.svg" />
        <div class="contact_in_right_text">
          <h5>Мы в Telegram</h5>
          <p>Отвечаем быстро</p>
        </div>
      </div>
    </div>
    <div class="pbg_img_position">
      <img class="img_1" src="/img/1.svg" />
      <img class="img_2" src="/img/2.svg" />
      <img class="img_3" src="/img/3.svg" />
      <img class="img_4" src="/img/4.svg" />
      <img class="img_5" src="/img/5.svg" />
      <img class="img_6" src="/img/6.svg" />
      <img class="img_7" src="/img/7.svg" />
      <img class="img_8" src="/img/8.svg" />
      <img class="img_9" src="/img/9.svg" />
      <img class="img_10" src="/img/10.svg" />
      <img class="img_11" src="/img/11.svg" />
      <img class="img_12" src="/img/12.svg" />
      <img class="img_13" src="/img/13.svg" />
      <img class="img_14" src="/img/14.svg" />
    </div>
  </div>
</template>

<style scoped>
#contact .pbg_img_position {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
}
#contact .pbg_img_position .img_2 {
  position: absolute;
  top: 0;
  left: 230px;
}
#contact .pbg_img_position .img_3 {
  position: absolute;
  top: 180px;
  left: 80px;
}
#contact .pbg_img_position .img_4 {
  position: absolute;
  top: 500px;
  left: 80px;
}
#contact .pbg_img_position .img_5 {
  position: absolute;
  top: 600px;
  left: 240px;
}
#contact .pbg_img_position .img_6 {
  position: absolute;
  top: 755px;
  left: 7px;
}
#contact .pbg_img_position .img_7 {
  position: absolute;
  z-index: 2;
  top: 800px;
  left: 340px;
}
#contact .pbg_img_position .img_8 {
  position: absolute;
  top: 10px;
  right: 282px;
}
#contact .pbg_img_position .img_9 {
  position: absolute;
  top: 570px;
  right: 20px;
}
#contact .pbg_img_position .img_10 {
  position: absolute;
  top: 120px;
  right: 11px;
}
#contact .pbg_img_position .img_11 {
  position: absolute;
  top: 608px;
  right: 176px;
}
#contact .pbg_img_position .img_12 {
  position: absolute;
  top: 828px;
  right: 408px;
}
#contact .pbg_img_position .img_13 {
  position: absolute;
  top: 824px;
  right: -14px;
}
#contact .pbg_img_position .img_14 {
  position: absolute;
  top: 353px;
  right: 194px;
}
#contact {
  position: relative;
  max-width: 1920px;
  padding-bottom: 100px;
}
#contact h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 87px;
  letter-spacing: -0.02em;
  padding-bottom: 17px;
  padding-top: 250px;
}
#contact p {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 26px;
  line-height: 35px;
  text-align: center;
  letter-spacing: -0.02em;
  padding-bottom: 65px;
}
#contact .registration {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 26px;
  line-height: 35px;
  letter-spacing: 0.015em;
  color: #ffffff;
  background: #0066ff;
  border-radius: 11px;
  max-width: 355px;
  max-height: 62px;
  padding: 15px 30px;
  margin-bottom: 205px;
}
#contact .contact_in {
  position: relative;
  z-index: 1;
  width: 895px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background: rgba(255, 255, 255, 0.43);
  backdrop-filter: blur(5px);
  border-radius: 20px;
  padding: 30px 50px;
  margin-bottom: 180px;
}
#contact .contact_in p {
  font-family: "Roboto", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 145.03%;
  color: #8aa0b4;
  max-width: 447px;
}
#contact .contact_in .contact_in_left h5 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 26px;
  line-height: 35px;
  letter-spacing: -0.01em;
  color: #203a54;
  margin-bottom: 20px;
}
#contact .contact_in .contact_in_right {
  display: flex;
  background: #ffffff;
  border: 1px solid #e4e4e4;
  border-radius: 15px;
  justify-content: space-around;
  align-items: center;
  max-width: 284px;
  height: 77px;
  padding: 10px 20px;
}
#contact .contact_in .contact_in_right h5 {
  font-family: "Roboto", sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 24px;
  line-height: 131.69%;
  color: #57a9da;
  padding-bottom: 0;
}
#contact .contact_in .contact_in_right .contact_in_right_text p {
  padding-bottom: 0;
}

@media (max-width: 1600px) {
    #contact .pbg_img_position .img_7 {
  position: absolute;
  z-index: 2;
  top: 800px;
  left: 150px;
}
    #contact .pbg_img_position .img_12 {
  position: absolute;
  top: 828px;
  right: 200px;
}
}
</style>
