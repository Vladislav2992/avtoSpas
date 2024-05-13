<template>
    <section class="steps" id="how-it-work">
        <div class="container">
            <h2 class="section__title">Как это работает</h2>
            <div class="wrapper">
                <div class="step">
                    <div class="counter">1</div>
                    <div class="counter-mobile">Шаг 1</div>
                    <p class="description">Создается заявка через Telegram бота, проходит модерацию</p>
                    <img src="/app.png" alt="">
                </div>
                <div class="step">
                    <div class="counter">2</div>
                    <div class="counter-mobile">Шаг 2</div>
                    <p class="description">Заявка публикуется <br> в региональный канал, ожидает исполнителя </p>
                    <img src="/app.png" alt="">
                </div>
                <div class="step">
                    <div class="counter">3</div>
                    <div class="counter-mobile">Шаг 3</div>
                    <p class="description">Находится исполнитель, едем спасать!</p>
                    <img src="/app.png" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="sass" scoped>
.steps
    background-image: url('../assets/img/steps-bg.png')
    background-size: cover
    background-position: center
    padding-top: clamp(30px, 7vw, 65px)
    padding-bottom: clamp(30px, 7vw, 45px)
    color: white
.section__title
    margin-bottom: 45px
.wrapper
    display: flex
    justify-content: space-between
    text-align: center
.step
    max-width: 400px
    width: 100%
    display: flex
    flex-direction: column    
    gap: 33px
    align-items: center

    img
        margin-top: auto
        width: 70%

    &:nth-child(3) .counter::after
        content: none
.counter
    width: 70px
    height: 70px
    border-radius: 100%
    display: flex
    align-items: center
    justify-content: center
    border: 1px solid white
    margin: 0 auto
    position: relative

    &::after
        content: ''
        position: absolute
        height: 1px
        width: 20vw
        top: 50%
        left: 9vw
        transform: translateY(-50%)
        background: white
.counter-mobile
    font-size: 20px
    font-weight: 700
    text-align: center
    display: none
.description
    font-size: clamp(16px, 5vw, 30px)
    line-height: 117%

@media(min-width: 1440px)
    .counter::after
        width: 250px
        left: 174%
@media(max-width: 860px) 
    .counter
        display: none
        &::after
        content: none
    .counter-mobile
        display: block
    .wrapper
        flex-direction: column
        align-items: center
        gap: 30px
    .step
        gap: 15px
    .section__title
        margin-bottom: 30px
</style>