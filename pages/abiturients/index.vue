<template>
    <div>
        <div class="main-abitur">
            <div class="title-abitur">
                <h2>Поступай в КФУ и учись здесь</h2>
            </div>
            <div class="abitbut-container">
                <div class="button-wrapper"><button>#Школьнику</button></div>
                <div class="button-wrapper"><button>#Иностранным гражданам</button></div>
                <div class="button-wrapper"><button>Подать документы</button></div>
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
                    <p>День открытых дверей: Институт математики и механики им. Н.И. Лобачевского  </p>
                </div>
            </div>
            </div>
        </div>
        <div class="guide-admission">
            <div class="guide-title"><h2>Процедура поступления</h2></div>
            <div class="menu-wrapper">
            <div class="contbut-guide" id="scroller">
                <div class="button-guide"><button>Бакалавриат/Спец</button></div>
                <div class="button-guide"><button class=" active">Магистратура</button></div>
                <div class="button-guide"><button>Аспирантура</button></div>
            </div>
        </div>
        </div>
        <div class="guide-desc">
            <div class="guide-item"><h2>Выбрать направление подготовки</h2></div>
            <div class="arrow"><img src="../../image/Vector (1).svg"></div>
            <div class="guide-item"><h2>Подать документы</h2></div>
            <div class="arrow"><img src="../../image/Vector (1).svg"></div>
            <div class="guide-item"><h2>Пройти вступительные испытания</h2></div>
            <div class="arrow"><img src="../../image/Vector (1).svg"></div>
            <div class="guide-item"><h2>Отслеживай конкурсные списки поступающих</h2></div>
            <div class="arrow"><img src="../../image/Vector (1).svg"></div>
            <div class="guide-item"><h2>Подай документы об образовании</h2></div>
            <div class="arrow"><img src="../../image/Vector (1).svg"></div>
            <div class="guide-item"><h2>Найти себя в приказе о зачислении</h2></div>
        </div>
        <div class="form">
        <div class="form-title">
            <h2>Оставь заявку и поступи <br> в лучший университет</h2>
        </div>
        <form>
            <label for="last-name">Фамилия</label>
            <input type="text" id="last-name">
            <label for="name">Имя</label>
            <input type="text" id="name">
            <label for="patronymic">Отчество</label>
            <input type="text" id="patronymic">
            <label for="date-birth">Дата рождения</label>
            <input type="text" id="date-birth">
            <div class="but-enter"><button>Поступить</button></div>
        </form>
    </div>

    </div>
</template>
<style>
.form{padding-bottom: 100px;}
.but-enter button{background: rgb(161, 31, 31);color: white;font-size: 1.5rem;font-family: Inter;font-weight: 400;border: 0;border-radius: 20px;padding: 20px 60px 20px 60px;}
input{min-height: 50px;border-radius: 10px;border: 0;width: 73.5%;}
.but-enter {padding-top: 40px;padding-bottom: 40px;}
form{display: flex;flex-direction: column;max-width: 540px;margin: 0 auto;background: rgb(0, 85, 144);align-items: center;border-radius: 10px;}
label{padding-top: 40px;font-size: 1.5rem;font-family: Inter;color: white;font-weight: 400;padding-bottom: 20px;}
.form-title h2{font-size: 2.5rem;font-family: Inter;font-weight: 400;text-align: center;}
.form-title{padding-bottom: 60px; display: flex;justify-content: center;}
    .guide-desc{padding-bottom: 100px;}
.arrow{padding: 18px 0 18px 0;}
.guide-desc{display: flex;flex-direction: column;align-items: center;}
.guide-item h2{font-size: 2.5rem;font-family: Inter;font-weight: 400;text-align: center;}
.guide-admission{padding-bottom: 40px;}
.menu-wrapper{overflow: hidden;width: 100%;}
.button-guide .active{background: rgb(0, 85, 144);color: white;}
.button-guide button{min-width:337.3px;font-size: 1.5rem;font-weight: 400;font-family: Inter;padding: 18px 10px 18px 10px;background: white;border: 1px solid rgb(4, 58, 106);border-radius: 20px;width: 100%;}
.contbut-guide{display: flex;max-width: 1100px;justify-content: space-between ;margin: 0 auto;overflow: auto;padding-bottom: 20px;
    margin-bottom: -20px;}
.guide-title{display: flex;justify-content: center;padding-bottom: 60px;}
.guide-title h2{font-size: 2.5rem;font-family: Inter;font-weight: 400;}
.calendar-abitur{padding-bottom: 104px;}
.cal-item{max-width: 336.92px;border-radius: 20px;height: 210px;}
.date{padding-bottom: 10px;padding-top: 10px;padding-left: 10px;}
.cal-desc{padding-top: 10px;padding-left: 10px;}
.cal-item:first-child{background-color: rgb(14, 89, 156);color: white;}
.date p,.cal-desc p {margin: 0;padding: 0;}
.cal-item:nth-child(2){border: rgb(4, 58, 106) 1px solid;}
.cal-item:last-child{border: rgb(4, 58, 106) 1px solid;background: rgb(229, 229, 229);}
.date,.cal-desc{font-size:  1.5rem;font-family: Inter;font-weight: 400;}
.cal-container{display: flex;max-width: 1100px;width: 100%;margin: 0 auto;justify-content: space-between;}
.cal-title{padding-top: 96px;padding-bottom: 60px;display: flex;justify-content: center}
.cal-title h2{font-size: 2.5rem;font-family: Inter;font-weight: 400;}
.main-abitur{background: rgb(0, 85, 144);padding-bottom: 170px;}
.abitbut-container{display: flex;flex-wrap: wrap-reverse;justify-content: center;max-width: 1288px;margin: 0 auto;}
.button-wrapper button{width: 100%;min-width: 634px;height: 99px; border-radius: 20px; background: rgb(4, 58, 106);
color: white;font-family: Inter;font-size: 2.6rem;border: 0;font-weight: 300;}
.title-abitur h2{color: white;font-size: 2.5rem;font-weight: 400;font-family: Inter;}
.title-abitur{padding-top: 155px;padding-bottom: 50px;display: flex;justify-content: center;}
.button-wrapper{padding-bottom: 25px;}
.button-wrapper:first-child{padding-right: 20px;}
@media screen and (max-width:1288px){
    .abitbut-container{flex-direction: column-reverse;}
    .button-wrapper{padding-left: 13.5px;padding-right: 13.5px;}
    .button-wrapper:first-child{padding-right: 13.5px;}
}
@media screen and (max-width:1055px) {
    .cal-container{flex-direction: column; height: 550px;align-items: center;}
    .cal-item {height: auto;max-width: 291px;}
    .cal-desc{padding-bottom: 10px;}
    .menu-wrapper{display: flex;justify-content: center;}
    .button-guide{padding-right: 20px;}
    
}
@media screen and (max-width:660px){
    .form{padding-bottom: 40px;}
    .but-enter {padding-left: 10px;padding-right: 10px;width: 100%;padding-bottom: 20px;padding-top: 10px;display: flex;justify-content: center;}
    .but-enter button{font-size:1rem;padding:0;border-radius: 7.5px;max-width:270px;height:40px;width: 100%;}
    input{min-height: 30px;}
    label{font-size: 1rem;}
    label:first-child{padding-top: 20px;}
    label{padding-top: 10px;padding-bottom:5px;}
    form{max-width: 290px}
    .form-title h2{font-size:1.125rem}
    .form-title{padding-bottom: 20px;}
    .guide-desc{padding-bottom: 40px;}
    .arrow img{width: 10px;}
    .arrow {padding: 0 3px 0 3px;}
    .guide-item h2{font-size: 1rem;}
    .guide-admission{padding-bottom: 20px;}
    .calendar-abitur{padding-bottom: 40px;}
    .guide-title{padding-bottom: 20px;}
    .button-guide button{font-size: 1rem;min-width: 200px;padding: 19px 0 19px 0;}
    .guide-title h2{font-size: 1.125rem;}
    .cal-title h2{font-size: 1.125rem;}
    .cal-title{padding-top: 40px;padding-bottom: 20px;}
    .cal-container{height: 440px}
    .title-abitur h2{font-size: 1.125rem;}
    .title-abitur{padding-top: 40px;padding-bottom: 20px;}
    .button-wrapper button{font-size: 1rem;min-width: 0;height: 60px;}
    .button-wrapper{padding-bottom: 10px}
    .main-abitur{padding-bottom: 30px;}
    .cal-desc{font-size: 1rem;padding-bottom: 23px;}
    .date{font-size: 1.125rem;}

}
</style>
<script>
export default{

    mounted()
    {
        let element=document.getElementById("scroller");
        element.scrollLeft=157;

    }
}
</script>