<script setup>
import AppBtn from '../components/AppBtn.vue'
</script>

<template>
    <div class="bot">
        <div class="container">
            <div class="bot-wrapper">
                <div class="bot__img">
                    <img src="/images/bot-img.png" alt="">
                </div>
                <div class="bot-texts">
                    <h3 class="bot__title title">Наличие <b> Телеграм Бота</b></h3>
                    <p class="bot__subtitle sub-title">Полный функционал мобильного приложения Al Chiroq доступен в телеграм-боте.
                        Заходите с любого устройства для того, чтобы получать ежедневные бонусы, а так же совершать
                        покупки
                        в магазине за заработанные коины.
                    </p>
                    <div class="bot__btn">
                        <app-btn />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.bot {
    background-image: url('/images/bot-bg.png');
    background-repeat: no-repeat;
    background-position-x: right;
    background-size: 10% auto;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    &__img {
        img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 43%;
    }

    &__subtitle {
        font-weight: 400;
        font-size: 16px;
        line-height: 24px;
        background: linear-gradient(145.27deg, #313331 -5.05%, #181716 105.01%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-fill-color: transparent;
        margin-top: 16px;
        margin-bottom: 40px;
    }
}
</style>