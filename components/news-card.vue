<template>
    <div class="card-container">
        <div class="image-wrapper"><img src="../image/news-img.png"></div>
        <div class="about-container">
            <div class="news-title">
                <p>КФУ стал участником выставки «Образование. Карьера»</p>
            </div>
            <div class="news-disc">
                <p>Свои учебные программы презентовали вузы России, а также Белоруссии и Казахстана.</p>
            </div>
        </div>
    </div>
</template>
<style scoped>
.card-container{display: flex;max-width: 786px; box-shadow: 2px 8px 4px 0px rgba(34, 60, 80, 0.25);border-radius:0px 15px 15px 0px;}
.news-title,.news-disc{font-size:1.5rem;font-family: Inter;font-weight: 400;color: rgb(4, 58, 106);padding-left: 10px;}
.news-disc{padding-top: 24px;}
.news-title{padding-top: 35px;}
p{padding: 0;margin: 0;}
@media screen and (max-width:600px){
    .card-container{flex-wrap: wrap;}
    .image-wrapper{width: 100%;}
    .image-wrapper img{width: 100%;}
    .news-disc,.news-title{font-size: 1rem;}
    .news-disc{padding-top: 10px;padding-bottom: 20px;}
}
</style>