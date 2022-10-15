<template>
    <!-- mana bu earnings component -->
    <div class="earnings">
        <div class="earnings_wrapper">
            <div class="earnings_in">
                <div class="earnings_title">
                    <img class="mx-auto" src="/img/logo.svg" alt="logo.svg">
                    <h1>Возможности для заработка</h1>
                </div>
                <div class="referral">
                    <div class="referral_in">
                        <h1>Реферальная программа</h1>
                        <div class="referall_percentage">
                            <h3>до</h3>
                            <h2>80%</h2>
                            <h3>навсегда</h3>
                        </div>
                        <div class="referall_img">
                            <img src="/img/referall_img.svg" alt="referall_img.svg">
                        </div>
                    </div>
                </div>
                <div class="seller">
                    <div class="seller_in">
                        <div class="seller_text">
                            <h1>Заработок на P2P</h1>
                            <p>Никакой игры на росте или падении цен, только гарантированный доход.</p>
                            <p>Станьте участником P2P-секции и зарабатывайте на комиссии.</p>
                            <a href="">Стать верифицированным продавцом →</a>
                        </div>
                        <div class="seller_img">
                            <img src="/img/seller_img.svg" alt="seller_img.svg">
                        </div>
                    </div>
                </div>
                <div class="services">
                    <div class="services_in">
                        <div class="services_text">
                            <h1>Мощный API<br> для ваших сервисов</h1>
                            <p>Подключаем обменники и другие сервисы.Получите доступ к общирному функционалу биржи и зарабатывайте с Rapira API.</p>
                            <a href="">Создать аккаунт c API ключами →</a>
                        </div>
                        <div class="services_img">
                            <img src="/img/services_img.svg" alt="services_img.svg">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* earnings start-------------------------------------- */
.earnings_wrapper{
    max-width: 1920px;
    padding: 0 30px;
    margin: 0 auto;
}
.earnings_in{
    max-width: 1700px;
    margin: 0 auto;
    margin-bottom: 25px;
}
.earnings_title{
    margin-top: 150px;
    text-align: center;
    margin-bottom: 80px;
}
.earnings_title h1{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 60px;
    line-height: 82px;
    text-align: center;
    background: linear-gradient(0deg, #181C1F, #181C1F), linear-gradient(92.21deg, rgba(0, 0, 0, 0) 15.92%, rgba(0, 0, 0, 0.098) 22.48%, rgba(0, 0, 0, 0) 33.25%, rgba(0, 0, 0, 0.0169387) 66.05%, rgba(0, 0, 0, 0.2) 86.13%), #FBFBFB;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.referral{
    margin-bottom: 25px;
}
.referral .referral_in{
    padding: 0px 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: linear-gradient(0deg, #1B1B1D, #1B1B1D), #FFFFFF;
    box-shadow: 0px 4px 86px rgba(16, 36, 66, 0.1);
    border-radius: 36px;
    overflow: hidden;
}
.referral .referral_in h1{
    max-width: 518px;
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    line-height: 119.66%;
    letter-spacing: -0.02em;
    background: linear-gradient(0deg, #FFFFFF, #FFFFFF), linear-gradient(88.17deg, #5C88E8 -2.53%, #DB2F4E 104.21%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.referall_percentage{
    text-align:  center;
}
.referall_percentage h3{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 45px;
    line-height: 114.5%;
    background: linear-gradient(0deg, #CCCCCC, #CCCCCC), linear-gradient(0deg, #FFFFFF, #FFFFFF), linear-gradient(88.17deg, #5C88E8 -2.53%, #DB2F4E 104.21%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;   
}
.referall_percentage h2{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 114px;
    line-height: 115%;
    letter-spacing: 0.01em;
    background: linear-gradient(95.96deg, #FFDA46 12.85%, #E17511 110.75%), linear-gradient(95.96deg, #3B8E26 12.85%, #78CF62 110.75%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;    
}
/* ----------------------------------------------------- */
.seller{
    margin-bottom: 25px;
}
.seller_in{
    background: radial-gradient(89.86% 463.02% at 89.86% 26.4%, rgba(255, 255, 255, 0.24) 0%, rgba(255, 255, 255, 0) 100%), #FFFFFF;
    background-blend-mode: overlay, normal;
    box-shadow: 0px 4px 86px rgba(16, 36, 66, 0.1);
    border-radius: 41px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.seller_text{
    padding: 50px 0px 50px 50px;
}
.seller_text h1{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 72px;
    line-height: 117%;
    letter-spacing: 0.02em;
    color: #000000;
    margin-bottom: 50px;
}
.seller_text p{
    max-width: 803px;
    margin-bottom: 50px;
    font-family: 'Roboto',sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 40px;
    line-height: 145%;
    letter-spacing: 0.02em;
    color: #000000;
}
.seller_text a{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 40px;
    line-height: 149%;
    color: #000000;
}
.seller_img img{
    padding: 50px 50px 50px 0;
}
/* ----------------------------------------- */
.services_in{
    background: linear-gradient(0deg, #FAFBFB, #FAFBFB), #FFFFFF;
    box-shadow: 0px 4px 86px rgba(16, 36, 66, 0.1);
    border-radius: 41px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.services_text{
    padding: 50px 0px 50px 50px;
}
.services_text h1{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 72px;
    line-height: 117%;
    letter-spacing: 0.02em;
    color: #000000;    
    margin-bottom: 40px;
}
.services_text p{
    font-family: 'Roboto',sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 40px;
    line-height: 145%;
    letter-spacing: 0.02em;
    color: #000000;
    margin-bottom: 60px;
}
.services_text a{
    font-family: 'Open Sans',sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 40px;
    line-height: 149%;
    color: #000000;
}
</style>