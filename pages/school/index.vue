<template>
    <div>
        <div class="main-abitur">
            <div class="title-abitur">
                <h2>Информация для школьников</h2>
            </div>
            <div class="abitbut-container">
                <div class="button-wrapper"><button>Олимпиады</button></div>
                <div class="button-wrapper"><button>Мероприятия</button></div>
                <div class="button-wrapper"><button>Подготовка к ЕГЭ/ОГЭ</button></div>
            </div>
        </div>
        <div class="calendar-abitur">
            <div class="cal-title">
                <h2>Календарь событий</h2>
            </div>
            <div class="cal-container">
                <div class="cal-item">
                    <div class="date">
                        <p>7.12</p>
                    </div>
                    <div class="cal-desc">
                        <p>День открытых дверей: Набережночелнинский
                            институт КФУ</p>
                    </div>
                </div>
                <div class="cal-item">
                    <div class="date">
                        <p>7.12</p>
                    </div>
                    <div class="cal-desc">
                        <p>День открытых дверей: Институт экологии, биотехнологии и природопользования </p>
                    </div>
                </div>
                <div class="cal-item">
                    <div class="date">
                        <p>13.12</p>
                    </div>
                    <div class="cal-desc">
                        <p>День открытых дверей: Институт математики и механики им. Н.И. Лобачевского </p>
                    </div>
                </div>
            </div>
        </div>
        <div class="school-title">
            <h2>Учись, открывай, действуй вместе с нами!</h2>
        </div>
        <div class="school-desc">
            <p>Если ты хочешь стать успешным в современном мире, то тебе нужно принять его правила: постоянно
                прокачивать себя в личностном росте!</p><br>
            <p>От твоего уровня знаний зависит не только, насколько свободно и уверенно ты будешь чувствовать себя в
                обществе, но и каковы твои шансы на поступление в вуз мечты.
                Идеальный способ прокачаться – начать участвовать в наших мероприятиях уже сейчас!</p>
        </div>
        <div class="offers">
            <div class="offers-title">
                <h2>Мы предлагаем</h2>
            </div>
            <div class="offers-cont">
                <div class="wrapper-offer">
                    <div class="arrow-pict"><img src="../../image/arrow_right_alt.png"></div>
                    <div class="desc-offer">
                        <p>повысить свой уровень знаний, подготовиться к предметным олимпиадам на очных и дистанционных
                            курсах Малого университета и курсах олимпиадной подготовки;</p>
                    </div>
                </div>
                <div class="wrapper-offer">
                    <div class="arrow-pict"><img src="../../image/arrow_right_alt.png"></div>
                    <div class="desc-offer">
                        <p>подготовиться вместе с нами к экзаменам на курсах подготовки к ОГЭ и ЕГЭ;</p>
                    </div>
                </div>
                <div class="wrapper-offer">
                    <div class="arrow-pict"><img src="../../image/arrow_right_alt.png"></div>
                    <div class="desc-offer">
                        <p>принять участие в Межрегиональных предметных олимпиадах КФУ и олимпиадах, проводимых вместе с
                            нашими партнерами (Советом Федераций, МФТИ, НИУ ВШЭ и другими), вошедших в Перечень
                            Российского
                            совета олимпиад школьников, которые помогут тебе поступить в КФУ или другой вуз России без
                            вступительных испытаний или приравнять твои результаты ЕГЭ к 100 баллам;</p>
                    </div>
                </div>
                <div class="wrapper-offer">
                    <div class="arrow-pict"><img src="../../image/arrow_right_alt.png"></div>
                    <div class="desc-offer">
                        <p>принять участие в других мероприятиях (Олимпиаде WINKID, Всероссийской (с международным
                            участием)
                            научной конференции учащихся им. Н.И. Лобачевского и др.), чтобы получить дополнительные
                            баллы
                            при поступлении в КФУ и попасть в Государственный информационный ресурс об одаренных детях
                        </p>
                    </div>
                </div>
                <div class="wrapper-offer">
                    <div class="arrow-pict"><img src="../../image/arrow_right_alt.png"></div>
                    <div class="desc-offer">
                        <p>почувствовать себя уже со школьной скамьи частью большого и дружного коллектива КФУ.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style>
.offers{padding-bottom: 20px;}
.arrow-pict{padding-right: 25px;}
.wrapper-offer{display: flex;align-items: center;padding-bottom: 25px;}
.offers-cont{display: flex;max-width: 1110px;flex-direction: column;margin: 0 auto;}
.desc-offer p{margin: 0;font-family: Inter;font-size: 1.5rem;font-weight: 400;}
.offers-title{display: flex;justify-content: center;padding-bottom: 94px;}
.offers-title h2{
    font-family: Inter;
    font-size: 2.5rem;
    font-weight: 400;
}
.school-title{
    display: flex;
    justify-content: center;
    padding-bottom: 87px;
}
.school-title h2{font-size: 2.5rem;font-family: Inter;font-weight: 400;text-align: center;}
.school-desc p{margin: 0;padding: 0;font-family: Inter;font-weight: 400;font-size: 1.5rem;}
.school-desc p:first-child{padding-bottom: 10px;}
.school-desc{padding-bottom: 195px;}
.school-desc{max-width:1105px;display: flex ;margin: 0 auto;text-align: center;flex-direction: column;}
@media screen and (max-width:660px){
    .offers{padding-bottom: 40px;}
    .offers-cont{min-height: 830px;justify-content: space-between;}
    .offers-title{padding-bottom: 20px;}
    .arrow-pict{display: none;}
    .desc-offer{padding-left: 10px;padding-right: 10px;padding-top: 5px;padding-bottom: 5px;}
    .wrapper-offer{width: 90%;border: solid 1px black;margin: 0 auto;padding-bottom: 0px;border-radius: 15px;}
    .desc-offer p{font-size: 1rem;}
    .offers-title h2{font-size: 1.125rem;}
    .school-title h2{font-size: 1.125rem;}
    .school-title{padding-bottom: 20px;padding-left: 15px;padding-right: 15px;}
    .school-desc p{font-size: 1rem;}
    .school-desc{padding-left: 15px;padding-right: 15px;padding-bottom: 40px;}
    
}
</style>