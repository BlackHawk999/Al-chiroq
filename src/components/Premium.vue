<script setup>
import AppBtn from "./AppBtn.vue"

</script>

<template>
    <div class="premium">
        <div class="container">
            <div class="premium-wrapper">
                <div class="premium-texts">
                    <h3 class="premium__title title">Al Chiroq <b>Premium</b></h3>
                    <p class="premium__subtitle sub-title">С Al Chiroq Premium вы получаете еще больше бонусов, а также ряд
                        дополнительных преимуществ, таких как выбор между интернет-трафиком или минутами.
                    </p>
                    <div class="premium-items">
                        <div class="premium-item">
                            <div class="premium-item__img">
                                <img src="/images/premium-byte.svg" alt="">
                            </div>
                            <div class="premium-item-texts">
                                <p class="premium-item__text">Интернет трафик</p>
                                <p class="premium-item__subtext">До 2000 МБ</p>
                            </div>
                        </div>
                        <div class="premium-item">
                            <div class="premium-item__img">
                                <img src="/images/premium-clock.png" alt="">
                            </div>
                            <div class="premium-item-texts">
                                <p class="premium-item__text">Дополнительные минуты</p>
                                <p class="premium-item__subtext">До 2000 минут</p>
                            </div>
                        </div>
                        <div class="premium-item">
                            <div class="premium-item__img">
                                <img src="/images/premium-green.png" alt="">
                            </div>
                            <div class="premium-item-texts">
                                <p class="premium-item__text">Пополнение баланса</p>
                                <p class="premium-item__subtext">до 50 000 сум</p>
                            </div>
                        </div>
                        <div class="premium-item">
                            <div class="premium-item__img">
                                <img src="/images/premium-gift.svg" alt="">
                            </div>
                            <div class="premium-item-texts">
                                <p class="premium-item__text">Большой шанс выиграть</p>
                                <p class="premium-item__subtext">Ценные призы</p>
                            </div>
                        </div>
                    </div>
                    <app-btn />
                </div>
                <div class="premium__img">
                    <img src="/images/premium-img.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.premium {
    background-image: url('/images/premium-main-bg.png');
    background-repeat: no-repeat;
    background-position: center;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 65px 0;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 50%;
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
    }

    &-items {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        row-gap: 16px;
        column-gap: 30px;
        margin-top: 24px;
        margin-bottom: 40px;
    }

    &-item {
        display: flex;
        align-items: center;

        &__img {
            margin-right: 16px;

            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }

        &-texts {
            display: flex;
            flex-direction: column;
        }

        &__text {
            font-weight: 400;
            font-size: 16px;
            line-height: 24px;
            background: linear-gradient(145.27deg, #313331 -5.05%, #181716 105.01%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }

        &__subtext {
            font-weight: 600;
            font-size: 20px;
            line-height: 24px;
            background: linear-gradient(145.27deg, #313331 -5.05%, #181716 105.01%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
    }

}
</style>