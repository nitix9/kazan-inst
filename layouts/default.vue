<template>
    <header>
        <nav>
        <div class="logo"><img src="..\image\logo.svg"></div>
        <div class="second-logo"><img src="..\image\priority.svg"></div>
        <div class="user-profile"><img src="..\image\lk.svg"> Личный кабинет</div>
        <div class="menu-items"><ul>
            <li>Студентам</li>
            <li>Абитуриентам</li>
            <li>Школьникам</li>
            <li>Здравохранение</li>
            <li>Об университете</li>
        </ul></div>
        </nav>
    </header>
    <slot/>
    <footer></footer>
</template>
<style>
html,body {padding: 0;margin: 0;}
header {background-color: rgb(0, 85, 144)}
</style>