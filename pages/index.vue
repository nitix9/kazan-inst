<template>
    <div>
        <div class="first-screen">
            <div class="title-container">
                <div class="main-title">
                    <h1>200 Лет</h1>
                </div>
                <div class="desc-title">
                    <h2>Знаний</h2>
                    <h2>Исследований</h2>
                    <h2>Традиций</h2>
                </div>
            </div>
        </div>
        <div class="news">
            <div class="title-screen">
                <h2>Новости</h2>
            </div>
            <div class="news-container">
                <div class="card-item">
                    <NewsCard />
                </div>
                <div class="card-item">
                    <NewsCard />
                </div>
            </div>
        </div>
        <div class="social-program">
            <div class="title-program">
                <h2>Наши программы</h2>
            </div>
            <div class="program-container">
                <div class="wrapper"><img src="/image/program1.png"></div>
                <div class="wrapper"><img src="/image/program2.png"></div>
                <div class="wrapper"><img src="/image/program3.png"></div>
                <div class="wrapper"><img src="/image/program4.png"></div>
            </div>
        </div>
        <div class="univin-num">
            <div class="num-title">
                <h2>Университет в цифрах</h2>
            </div>
            <div class="num-container">
                <div class="num-wrap">
                    <div class="pict-wrap"><img src="/image/number4.svg"></div>
                    <div class="desc-pic">
                        <p>более 47 000
                            общий контингент</p>
                    </div>
                </div>
                <div class="num-wrap">
                    <div class="pict-wrap"><img src="/image/number2.svg"></div>
                    <div class="desc-pic">
                        <p>более 400
                            учебных лабораторий</p>
                    </div>
                </div>
                <div class="num-wrap">
                    <div class="pict-wrap"><img src="/image/number3.svg"></div>
                    <div class="desc-pic">
                        <p>более 16 000
                            мест в общежитии</p>
                    </div>
                </div>
                <div class="num-wrap">
                    <div class="pict-wrap"><img src="/image/number1.svg"></div>
                    <div class="desc-pic">
                        <p>более 600
                            академических программ</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style>
.program-container .wrapper:last-child,.program-container .wrapper:nth-child(3){
    padding-bottom: 35px;
}
.desc-pic p{padding: 0;margin: 0;}
.pict-wrap{padding-bottom: 37px;}
.univin-num{padding-bottom: 104px;}
.num-wrap{max-width: 160px;width: 100%;}
.num-container{display: flex;justify-content: center;max-width: 1005px;justify-content: space-between;margin: 0 auto    ;padding: 0 20px 0 20px;}
.desc-pic{font-size: 1.25rem;font-family: Inter;font-weight: 400;}
.num-title{display: flex;justify-content: center;padding-top: 81px;padding-bottom: 76px;}
.num-title h2 {font-family: Inter;font-weight:400 ;font-size:2.5rem ;}
.title-program{padding-top: 15px;display: flex;justify-content: center;padding-bottom: 65px;}
.title-program h2 {font-family: Inter;color: white;font-size: 2.5rem;font-weight: 300;}
.wrapper{padding-bottom: 42px;}
.program-container{display: flex;justify-content: space-between;flex-wrap: wrap;margin: 0 auto;max-width: 1111px;padding: 0 10px 0 10px;}
.social-program{background-color: rgb(0, 85, 144);}
.card-item{padding-bottom: 40px}
.news-container .card-item:last-child{padding-bottom: 75px;}
.title-screen{display: flex;justify-content: center;padding-top: 68px;padding-bottom: 40px;}
.title-screen h2{color: rgb(4, 58, 106);font-family: Inter;font-weight: 400;font-size: 2.5rem;}
.news-container{display: flex;flex-direction: column;align-items: center;}
.first-screen{background:url("\image\firstscreen.png") no-repeat,linear-gradient(45deg, rgba(0,94,159,1) 0%,rgba(0,94,161,1) 18%,rgba(37,88,165,1) 28%,rgba(37,88,165,1) 28%,rgba(37,88,165,1) 51%,rgba(0,59,111,1) 55%,rgba(8,50,89,1) 64%,rgba(0,59,111,1) 97%);;width: 100%;height: 675px;display: flex;flex-direction: column;align-items: center;background-position: center center;}
.title-container{display: flex;flex-direction: column;align-items: center;height: 410px;justify-content: space-between;min-width: 757px;padding-left: 25px;}
.desc-title{display: flex;justify-content: space-between;width: 100%;}
.main-title{padding-top: 64px;}
.main-title h1{font-family: Inter;font-weight: 700;color: white;font-size:  2.5rem;}
.desc-title h2{font-family: Inter;font-weight: 700;color: white;font-size:  2.5rem;}
h1,h2{margin: 0;padding: 0;}
@media screen and (max-width:840px){
    .card-item{padding-left: 20px;padding-right: 20px;}
}
@media screen and (max-width:800px) {
    .first-screen{background-size: contain;
    background-repeat: no-repeat;
    width: 100%;
    height: 0;
    padding-top: 45%;}
    .title-container{display: none; }
}
@media screen and (max-width:950px) {
    .social-program{border-radius: 15px;}
    .program-container{flex-direction: column;align-items: center;}
    .wrapper{padding-bottom: 10px;}
    .wrapper:last-child{padding-bottom: 20px;}
    .title-program{padding-bottom: 20px;}

    .wrapper img{width: 100%;}
    
}
@media screen and (max-width:700px){
    .num-container{flex-direction: column;align-items: center;}
    .desc-pic{text-align: center;font-size: 1rem;padding-bottom: 10px;}
    .univin-num{padding-bottom: 40px;}
    .num-title{padding-top: 40px;padding-bottom: 20px;}
}
@media screen and (max-width:490px){
    .num-title h2{font-size: 1.125rem}
    .title-program h2{font-size: 1.125rem;padding-top: 10px;}
    .title-screen h2{font-size: 1rem;}  
}
@media screen and (max-width:600px) {

    .card-item{padding-left: 10px;padding-right: 10px;}
    .title-screen{display: flex;justify-content: center;padding-top: 40px;padding-bottom: 20px;}

}
</style>