<template>
    <section class="hero">
        <div class="container">           
            <h1 class="main__title">АвтоСпас - быстрая помощь на дороге и вне дорог через региональные сообщества в Telegram.</h1>
            <div class="img">
                <img src="/main-img.png" alt="">
            </div>
            <p class="description">Сломались на дороге, застряли в грязи, нужна эвакуация с леса или бездорожья? <br> Создайте заявку, и её увидят все участники сообщества в вашем регионе.</p>
            <button class="btn">Да, создать заявку</button>                 
        </div>
    </section>
</template>

<style lang="sass" scoped>
.hero
    background-image: url('../assets/img/main-bg.jpg')
    background-size: cover
    background-position: center
    display: flex
    align-items: center
    justify-content: center
    color: white
    padding-top: clamp(25px, 8vw, 100px)
    padding-bottom: clamp(30px, 8vw, 100px)
.container
    display: grid
    grid-template-columns: .6fr .4fr
    align-items: center

.main__title
    font-size: clamp(24px, 6vw, 50px)
    line-height: 124%
    margin-top: 15px
    // position: relative
    // z-index: 1
    // &::before
    //     content: ''
    //     position: absolute
    //     top: -100%
    //     left: 50%
    //     transform: translate(-50%)       
    //     width: 800px
    //     height: 800px       
    //     background-image: url('../assets/img/radial.svg')
        z-index: 0
.description
    font-size: clamp(16px, 4vw, 30px)
    line-height: 124%
    margin-top: -21px
.img
    grid-column: 2/3
    grid-row: 1/4
    display: flex

    img
        margin-left: auto
    
@media(max-width: 1024px)
    .container
        grid-template-columns: 1fr
        gap: 20px
    .img
        grid-column: 1/2
        grid-row: auto

        img
            margin: 0 auto
    .description,
    .main__title
        margin: 0
    .btn
        margin: 0 auto
</style>