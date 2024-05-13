<template>
    <div class="advantages">
        <div class="container">
            <h2 class="section__title">Чем удобен сервис в Telegram? </h2>

            <div class="wrapper">
                <div class="advantage">
                    <span class="number">1</span>
                    <p>Легко создать заявку. Не надо скачивать сторонние приложения.Все в Telegram!</p>
                </div>
                <div class="advantage">
                    <span class="number">2</span>
                    <p>Удобное взаимодействие (возможность оставлять комментарии и следить за статусом заявки).</p>
                </div>
                <div class="advantage">
                    <span class="number">3</span>
                    <p>Быстрое распространение информации в режиме реального времени.</p>
                </div>
                <div class="advantage">
                    <span class="number">4</span>
                    <p>Доступность 24/7. Пользователи могут получать информацию в любое время.</p>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="sass" scoped>
.advantages
    padding-top: clamp(30px, 7vw, 65px)
    padding-bottom: clamp(30px, 7vw, 52px)
.section__title
    margin-bottom: 40px
.wrapper
    display: grid
    grid-template-columns: repeat(4, 1fr)
    gap: 20px
.advantage
    display: flex
    flex-direction: column
    gap: 20px
.number
    font-size: clamp(50px, 9vw, 100px)
    line-height: 120%
    color: var(--red)
p
    line-height: 124%
@media(max-width: 860px)
    .wrapper
        grid-template-columns: 1fr 1fr
@media(max-width: 500px)
    .wrapper
        grid-template-columns: 1fr
    .advantage
        flex-direction: row
</style>