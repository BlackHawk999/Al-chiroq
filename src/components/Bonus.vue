<script setup>
import AppBtn from './AppBtn.vue';

</script>

<template>
    <div class="bonus">
        <div class="container">
            <div class="bonus-wrapper">
                <div class="bonus__img">
                    <img src="/images/bonus-img.png" alt="">
                </div>
                <div class="bonus-texts">
                    <h3 class="bonus__title title">Многоуровневая <b>бонусная система</b>для пользователей</h3>
                    <p class="bonus__subtitle sub-title">Наше приложение раздаёт реальные призы каждый день самым активным
                        пользователям. Повышайте ваш уровень и получайте шанс выигрывать самые ценные из призов.
                    </p>
                    <div class="bonus__btn">
                        <app-btn />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.bonus {
    background-color: #fff;

    &-wrapper {
        display: flex;
        align-items: center;
        padding: 36px 0;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 45%;
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