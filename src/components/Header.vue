<template>
    <header class="header">
        <div class="container">
            <div class="logo">
                <a href="/">
                    <img src="/logo.svg" alt="АвтоСпас">
                </a>
            </div>

            <nav class="menu">
                <ul class="menu__list">
                    <li class="item"><a href="#community-help">Для кого?</a></li>
                    <li class="item"><a href="#how-it-work">Как работает?</a></li>
                    <li class="item"><a href="#community-tg">Мы в Telegram</a></li>
                </ul>
                <button class="btn">Нужна помощь!</button>
            </nav>
        </div>
    </header>
</template>

<style lang="sass" scoped>
.header
    padding: 5px 0
    background: var(--red)
.container
    display: flex
    justify-content: space-between
    align-items: center 
    height: 100%
.logo
    width: clamp(35px, 7vw, 56px)
.menu
    color: white
    display: flex
    align-items: center 
    gap: 30px
.menu__list
    display: flex
    gap: clamp(10px, 3vw, 30px)
    font-size: clamp(14px, 3vw, 16px)

.btn
    border-color: white
    padding: 10px 20px
    width: fit-content
    font-size: 12px
    border-radius: 5px

@media (max-width: 786px)
    .header
        height: 50px
    .btn
        display: none
    
</style>