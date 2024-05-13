<template>
<section class="community" id="community-help">
    <div class="container">
        <h2 class="section__title">Сообщество помогает</h2>
        <ul class="list">
            <li class="item">
                <div class="img"><img src="/img.jpg" alt=""></div>
                <h3 class="title">Внедорожная эвакуация</h3>
                <p class="description">Застряли в поле, в луже в лесу, съехали в кювет. Застряли на раскисшей дороге по пути на дачу или вовсе в песке на пляже или глине у озера.</p>
            </li>
            <li class="devider"></li>
            <li class="item">
                <div class="img"><img src="/img.jpg" alt=""></div>
                <h3 class="title">Не можете проехать</h3>
                <p class="description">Если необходимо подвезти инструмент, топливо, провиант или людей в труднодоступные места.</p>
            </li>
            <li class="devider"></li>
            <li class="item">
                <div class="img"><img src="/img.jpg" alt=""></div>
                <h3 class="title">Помощь на дороге</h3>
                <p class="description">Cел аккумулятор, не заводится техника. Нужно отбуксировать машину. Попали в ливнёвку или канаву. Сообщество поможет!</p>
            </li>
        </ul>
        <div class="buttons">
            <button class="btn">Создать заявку</button>
            <button class="btn btn_white">Хочу помогать</button>
        </div>
    </div>
</section>    
</template>
<style lang="sass" scoped>
.community
    padding-top: clamp(30px, 7vw, 67px)
    padding-bottom: clamp(30px, 7vw, 60px)
.buttons
    display: flex
    gap: 25px
    justify-content: center
.section__title
    margin-bottom: 45px
.list    
    display: flex
    margin-bottom: 40px
    justify-content: space-between
    gap: 7px
.item
    max-width: 350px
    width: 100%
.devider
    width: 1px
    background: var(--red)
.img
    width: 100%
    overflow: hidden
    border-radius: 10px
    margin-bottom: 24px

    img
        width: 100%
.title
    font-weight: 600
    font-size: clamp(20px, 4vw, 26px)
    margin-bottom: clamp(8px, 4vw, 20px)
.description
    line-height: 120%    
@media(max-width: 786px)
    .section__title
        margin-bottom: 25px
    .list
        flex-direction: column
        gap: 25px
        margin-bottom: 25px
    .devider
        display: none
    .item
        max-width: 100%
    
    
</style>