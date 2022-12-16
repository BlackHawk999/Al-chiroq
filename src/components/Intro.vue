<script setup>
import AppLinks from '../components/AppLinks.vue'

</script>
<template>
    <div class="intro">
        <div class="container">
            <div class="intro-wrapper">
                <div class="intro-texts">
                    <h1 class="intro__title"><b>Al Chiroq</b> это интерактивная платформа которая позволяет получать
                        различные
                        бонусы!
                    </h1>
                    <p class="intro__texts">Приложение Al Chiroq предоставляет абонентам различные призы, бонусные
                        пакеты, а также способствует повышению лояльности абонентов оператора и уменьшению оттока вместе
                        с функцией привлечения дополнительных источников дохода.
                    </p>
                    <div class="intro-app">
                        <app-links />
                    </div>
                </div>
                <div class="intro__img">
                    <img src="/images/intro-img.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.intro {
    padding: 90px 0;
    min-height: 100vh;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 100%;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 50%;
    }

    &__title {
        font-style: normal;
        font-weight: 600;
        font-size: 40px;
        line-height: 48px;
        background: linear-gradient(148.86deg, #7243A0 -3.27%, #5B2D82 102.82%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-fill-color: transparent;
        margin-bottom: 16px;

        b {
            background: linear-gradient(145.66deg, #FCA305 -2.12%, #FF8130 101.98%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
    }

    &-app {
        margin-top: 50px;
    }

}
</style>