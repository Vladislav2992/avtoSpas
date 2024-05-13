<template>
    <section class="community" id="community-tg">
        <div class="container">
            <h2 class="section__title">Сообщество в Telegram</h2>
            <div class="wrapper">
                <div class="item">
                    <h3 class="title">Новости сообщества</h3>
                    <p>В этом канале мы делимся интересными и полезными историями нашей деятельности. Сообщаем про обновления сервиса. А так же проводим конкурсы среди участников сообщества АвтоСпас.</p>
                    <button class="btn_gray">Смотреть</button>
                </div>
                <div class="item">
                    <h3 class="title">Telegram Чат-бот</h3>
                    <p>Основной инструмент для создания заявок, получения уведомлений о заявках рядом и участия в реферальной программе сообщества АвтоСпас.</p>
                    <button class="btn_gray">Перейти в бота</button>
                </div>
                <div class="item">
                    <h3 class="title">Список регионов</h3>
                    <p>На данный момент сообщество присутствует в 20 самых населённых регионах страны. Найти свой регион можно в списке Telegram бота.</p>
                    <button class="btn_gray">Открыть список</button>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="sass" scoped>
.community
    background-image: url('../assets/img/community-bg.jpg')
    background-size: cover
    background-position: center
    padding-top: clamp(30px, 7vw, 65px)
    padding-bottom: clamp(30px, 7vw, 50px)
    color: white
.section__title
    margin-bottom: clamp(20px, 5vw, 55px)
.wrapper
    display: grid
    grid-template-columns: 1fr 1fr 1fr
    gap: 20px
.item
    padding: 30px
    backdrop-filter: blur(60px)
    box-shadow: inset 0 0 50px 0 rgba(0, 0, 0, 0.25), inset 0 -2px 4px 0 rgba(0, 0, 0, 0.25), inset 0 2px 2px 0 rgba(0, 0, 0, 0.25)
    background: linear-gradient(180deg, rgba(217, 217, 217, 0.1) 14%, rgba(115, 115, 115, 0.1) 100%)
    border-radius: 10px
    display: flex
    align-items: center
    justify-content: center
    flex-direction: column
    text-align: center
.title
    font-size: clamp(20px, 3vw, 30px)
    margin-bottom: 22px
p 
    font-size: clamp(14px, 2vw, 18px)
    margin-bottom: 37px
    line-height: 120%
.btn_gray
    background: #47443D
    border: none
    border-radius: 10px
    color: white
    font-size: clamp(12px, 3vw, 20px)
    padding-top: clamp(12px, 3vw, 20px)
    padding-bottom: clamp(12px, 3vw, 20px)
    width: clamp(167px, 21vw, 261px)
    margin-top: auto
    transition: background .3s

    &:hover
        background: #2f2d28 

@media(max-width:950px)
    .wrapper
        grid-template-columns: 1fr
        gap: 15px
@media(max-width:500px)
    .item
        padding: 20px 25px
    p 
        margin-bottom: 15px
</style>