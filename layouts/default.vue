<template>
    <header>
        <nav>
            <div class="container-head">
                <div class="head-menu">
                    <div class="logo"><img src="..\image\logo.svg"></div>
                    <div class="second-logo"><img src="..\image\priority.svg"></div>
                    <div class="burger-container">
                        <div @click="getClassStatus" class="burger" :class="{ active: isActive }"><span></span></div>
                    </div>
                    <div class="user-profile"><img src="..\image\lk.svg"> Личный кабинет</div>
                </div>
            </div>
            <div class="container-mobile-menu " :class="{open:isActive}">
                <div class="menu-items" :class="{open:isActive}">
                    <ul>
                        <div class="menu-item">
                            <li>Студентам</li>
                        </div>
                        <div class="menu-item">
                            <li>Абитуриентам</li>
                        </div>
                        <div class="menu-item">
                            <li>Школьникам</li>
                        </div>
                        <div class="menu-item">
                            <li>Здравохранение</li>
                        </div>
                        <div class="menu-item">
                            <li>Об университете</li>
                        </div>
                        <div class="menu-item">
                            <li>
                                <div class="user-profile-mobile"><img src="..\image\lk.svg"> Личный кабинет</div>
                            </li>
                        </div>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
    <slot />
    <footer>
        <div class="title-footer">
            <h2>Контакты</h2>
        </div>
        <div class="contacts-container">
            <div class="contact-item">
                <p>Приемная комиссия</p>
                    <p>420 008 Казань, Кремлевская 35</p>
                <p class="number">8 800 234 92 75</p>
                <p class="mail">priem@kpfu.ru</p>
            </div>
            <div class="contact-item">
                <p>Справочная</p>
                    <p>420 008 Казань, Кремлевская 18</p>
                <p class="number">8 843 233 71 09</p>
            </div>
            <div class="contact-item">
                <p>Управление кадров</p>
                <p>420 008 Казань, Кремлевская 18</p>
                <p class="mail">work@kpfu.ru</p>
            </div>
            <div class="contact-item">
                <p>Прием иностранных граждан</p>
                <p>420 008 Казань, Кремлевская 18</p>
                <p class="number">8 843 233 70 27</p>
                <p class="mail">admission@kpfu.ru</p>
            </div>
        </div>
        <div class="container-lcont">
        <div class="last-contacts">
            <div class="contact-item">
                <p>Управление документооборота и контроля</p>
                <p>420 008 Казань, Кремлевская 18</p>
                    <p class="number">8 843 292 72 16</p>
                    <p class="mail">public.mail@kpfu.ru</p>
            </div>
            <div class="contact-item">
                <p>Горячая линия по вопросам приема и обучения инвалидов и лиц с ОВЗ
                    </p>
                <p>8 843 206 52 94 доб. 8228</p>
            </div>
        </div>
    </div>
    </footer>
</template>
<style>
@font-face {
    font-family: Inter;
    src: url("../fonts/Inter_18pt-Regular.ttf");
    font-weight: 400;
}
@font-face {
    font-family: Inter;
    src: url("../fonts/Inter_28pt-Regular.ttf");
    font-weight: 401;
}
@font-face {
    font-family: Inter;
    src: url("../fonts/Inter_18pt-Light.ttf");
    font-weight: 300;
}
@font-face {
    font-family: Inter;
    src: url("../fonts/Inter_28pt-Light.ttf");
    font-weight: 301;
}

.container-lcont{display: flex;justify-content: center;padding-top: 15px;}
.last-contacts{display: flex;justify-content: space-between;}
.last-contacts div:last-child{max-width: 324px;padding-left: 20px;}
footer{background-color: rgb(0, 85, 144);}
.title-footer{display: flex;justify-content: center;padding-top:16px;}
.contacts-container{display: flex;flex-wrap: wrap;justify-content: space-between;padding:40px 40px 0 40px;}
.title-footer h2{color: white;font-family: Inter;font-weight: 300;font-size: 2.5rem;margin: 0;padding: 0;}
.contact-item{font-family: Inter;color: white;padding-bottom: 15px;}
.contact-item p{margin: 0;padding-bottom: 0;font-weight:300;font-size:1.25rem ;}
.mail, .number{padding-top: 24px;}
.burger-container{display: none;}
html,body {padding: 0;margin: 0;}
.menu-items ul div:last-child{display: none;}
.container-head{justify-content: center;}
header {background-color: rgb(0, 85, 144)}
.user-profile img{padding-right: 10px;}
.user-profile{display:flex;align-items: center;}
.user-profile-mobile{display: none;}
li{list-style-type: none; }
.burger {
    display: none;
    position: relative;
    z-index: 50;
    align-items: center;
    justify-content: flex-end;
    width: 30px;
    height: 18px;
}
.burger span {
    height: 2px;
    width: 100%;
    transform: scale(1);
    background-color: white;
}
.burger::before, .burger::after{
    content: '';
    position: absolute;
    height: 2px;
    width: 100%;
    background: white;
    transition:all 0.3s ease 0s;
}
.burger::before {
    top: 0;
}

.burger::after {
    bottom: 0;
}
.burger.active span{transform: scale(0);}
.burger.active::before{
    top:50%;
    transform: rotate(-45deg) translate(0,-50%);
}
.burger.active::after{
    bottom: 50%;
    transform: rotate(45deg) translate(0,50%);
}
.menu-items {background-color: rgb(4, 58, 106);}
.menu-items ul {
    display: flex;
    font-family: Inter;
    color: white;
    margin: 0;
    justify-content: space-between;
    align-items: center;
    font-size: 1.5rem;
    font-weight: 300;
    padding: 0.5% 7.2% 0.5% 7.2%;
}
.open{
    display: flex !important;
}
.head-menu{display: flex;justify-content: space-between;align-items: center;
padding: 0.9% 4.3% 0.3% 4.3%;}
.user-profile{color: white;font-family: Inter;font-weight: 300;}
@media screen and (max-width:1100px) {
.menu-items ul {font-size: 1.2rem;}
}
@media screen and (max-width:830px) {
.menu-items ul {font-size: 1rem;}
}
@media screen and (max-width:760px) {
    .title-footer h2{font-size: 1.125rem;}
    .container-lcont{padding: 0px 15px 0px 15px;}
    .last-contacts {text-align: center;}
    .last-contacts div:last-child{padding-left: 0;}
    .contact-item{display: flex;flex-direction: column;align-items: center;padding-bottom: 10px;}
    .contact-item p {font-size: 1rem;}
    .number,.mail{padding: 0;}
    .last-contacts{flex-direction: column;}
    .contacts-container{flex-direction: column;padding: 20px 15px 0px 15px;}
    .menu-items ul div:last-child{display: flex;}
    .burger-container{display: flex;}
    .user-profile-mobile img {padding-right: 10px;}
    .user-profile-mobile{align-items: center;}
.menu-items {background-color: rgb(0, 85, 144);}
.container-mobile-menu{display: none;justify-content: flex-end;}
.user-profile-mobile{display: flex;}
.menu-items{position: absolute;border-bottom-left-radius: 30px;}
.menu-item {width: 100%;text-align: center;border-bottom: solid white;}
.menu-items ul {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 0;
padding: 10px;font-size: 1.25rem; transform: rotate(180deg);}
.menu-items ul li {transform: rotate(-180deg);padding: 20px 0;}
.menu-items ul div:last-child{border-bottom:0px}
.second-logo{display: none;}
.user-profile{display: none;}
.burger{display: flex;}
}
</style>
<script>
export default{
    data() {
        return{
            isActive:false,
        }
    },
    methods:{getClassStatus(){
        if (this.isActive){
            this.isActive=false;
        }
        else {
            this.isActive=true;
        }
    }}
}
</script>