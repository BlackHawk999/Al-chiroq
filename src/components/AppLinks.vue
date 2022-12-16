<template>
    <div class="app-wrapper">
        <a href="http://youtube.com/Elyor Sadulaev" target="_blank" rel="noopener noreferrer" class="app__link">
            <img src="/images/intro-app.png" alt="">
        </a>
        <a href="http://youtube.com/Elyor Sadulaev" target="_blank" rel="noopener noreferrer" class="app__link">
            <img src="/images/intro-app-2.png" alt="">
        </a>
        <a href="http://youtube.com/Elyor Sadulaev" target="_blank" rel="noopener noreferrer" class="app__link">
            <img src="/images/intro-bot.png" alt="">
        </a>
    </div>
</template>

<style lang="scss">
.app {
    &-wrapper {
        display: flex;
        align-items: center;

    }

    &__link:not(:last-child) {
        margin-right: 24px;
    }

}
</style>