<template>
  <header>
    <div class="header-top">
      <div class="header-top-in">
        <div class="grid grid-cols-8 justify-center">
          <div
            class="
              lg:col-span-4
              md:col-span-5
              flex
              justify-between
            "
          >
            <img src="/img/logo.svg" alt="" />
            <ul class="flex header-link items-center">
              <li><a href="#">Главная</a></li>
              <li><a href="#">Торговля</a></li>
              <li><a href="#">Пополнение и вывод P2P</a></li>
            </ul>
          </div>
          <div
            class="lg:col-span-4 md:col-span-3 flex justify-end items-center"
          >
            <router-link class="access" to="/">Вход</router-link>
            <router-link class="flex sign-up" to="/"
              >Регистрация <img class="ml-2" src="/img/header_next_icon.svg" alt=""
            /></router-link>
            <div class="dropdown">
              <div class="dropdown__skeleton flex items-center">
                <div class="dropdown__selected dropdown__option">
                  <img
                    src="/img/rus-flag.svg"
                    alt="United Kingdom"
                  /><span>Русский</span>
                </div>

                <img class="ml-2" src="/img/lang-select-icon.svg" alt="" />
              </div>

              <div class="dropdown__options">
                <div class="dropdown__option">
                  <img
                    src="/img/rus-flag.svg"
                    alt="United Kingdom"
                  /><span>Русский</span>
                </div>
                <div class="dropdown__option">
                  <img
                    src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/237/flag-for-united-states_1f1fa-1f1f8.png"
                    alt="U.S."
                  /><span>U.S.</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="header-bottom">
      ⚠️️ Технические работы на сайте 17.11.2022 с 01:00 до 03:00 по МСК / 🔥
      Новая валюта USDC уже на сайте Смотреть все новости
    </div>
  </header>
</template>

<script>
export default {
  name: "HelloWorld",

  mounted() {
    console.clear();

    const dropdowns = document.querySelectorAll(".dropdown");

    dropdowns.forEach((dropdown) => {
      dropdown.addEventListener("click", (e) => {
        dropdown.classList.toggle("dropdown__options--visible");
      });

      dropdown
        .querySelectorAll(".dropdown__options .dropdown__option")
        .forEach((opt) => {
          opt.addEventListener("click", (e) => {
            dropdown.querySelector(".dropdown__selected").innerHTML =
              opt.innerHTML;
          });
        });
    });
  },
};
</script>

<style scoped>
header{
  position: relative;
  z-index: 3;
}
.header-top {
  max-width: 1920px;
  margin: 0 auto;
  padding: 20px 30px;
  position: relative;
  z-index: 2;
}
.header-top-in{
  max-width: 1700px;
  margin: 0 auto;
}
.header-link a {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  /* identical to box height */
  letter-spacing: -0.02em;

  color: #292929;
}
.header-link li {
  margin-left: 30px;
}
.access {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 21px;
  color: #000000;
}
.sign-up {
  background: linear-gradient(0deg, #000000, #000000), #005ff9;
  border-radius: 3px;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 21px;
  padding: 6px 13px;
  color: #ffffff;
  margin: 0 35px 0 25px;
}
.dropdown {
  position: relative;
  z-index: 3;
}
.dropdown__options--visible .dropdown__options {
  animation: showit 0.35s forwards ease-out;
}
.dropdown__skeleton {
  position: relative;
  transition: box-shadow 0.2s cubic-bezier(0.17, 0.67, 0.83, 0.67);
  cursor: pointer;
  user-select: none;
}
.dropdown__skeleton label {
  color: #9297ab;
  font-size: 0.8rem;
  letter-spacing: 0.64px;
  margin-bottom: 8px;
  display: block;
  cursor: pointer;
}
.dropdown__option {
  display: flex;
  align-items: center;
}
.dropdown__option span {
  margin-left: 10px;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  display: flex;
  align-items: center;
  letter-spacing: -0.02em;
  color: #000000;
}
.dropdown__arrow::before,
.dropdown__arrow::after {
  --angle: 40deg;
  content: "";
  width: 12px;
  background-color: #5e6582;
  display: block;
  padding: 1px;
  border-radius: 2px;
  position: absolute;
}
.dropdown__arrow::before {
  transform: rotate(var(--angle));
}
.dropdown__arrow::after {
  transform: rotate(calc(var(--angle) * -1));
  margin-left: 8px;
}
.dropdown__options {
  position: absolute;
  top: 110%;
  right: 0;
  border: 2px solid #dbe0f5;
  border-radius: 5px;
  padding: 20px 10px;
  background-color: #fff;
  transform: scale(0);
  z-index: 2;
  margin-top: 10px;
}
@keyframes showit {
  0% {
    transform: scale(0);
  }
  70% {
    transform: scale(1.05);
  }
  80% {
    transform: scale(0.95);
  }
  100% {
    transform: scale(1);
  }
}
.dropdown__options .dropdown__option {
  padding: 6px 10px;
  transition: background-color 0.2s ease-in-out, opacity 0.2s ease-in-out;
  cursor: pointer;
  opacity: 0.7;
  border-radius: 5px;
}
.dropdown__options .dropdown__option:not(:last-child) {
  margin-bottom: 15px;
}
.dropdown__options .dropdown__option:hover {
  background-color: #eee;
  opacity: 1;
}
.dropdown__options .dropdown__option--selected {
  opacity: 1;
}
.dropdown__options::before {
  content: "";
  position: absolute;
  bottom: calc(100% - 3px);
  right: 20px;
  height: 10px;
  width: 10px;
  background-color: #fff;
  border-top: 2px solid #dbe0f5;
  border-left: 2px solid #dbe0f5;
  transform: rotate(45deg);
}

*,
*::after,
*::before {
  box-sizing: border-box;
}

.dropdown img {
  max-width: 26px;
  display: block;
}
.header-bottom {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  text-align: center;
  letter-spacing: -0.02em;
  color: #535353;
  background: rgba(255, 255, 255, 0.2);
  padding: 10px 0;
  position: relative;
}
</style>
