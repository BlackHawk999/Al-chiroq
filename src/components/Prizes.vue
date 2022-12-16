<script setup>
import AppBtn from './AppBtn.vue';

</script>

<template>
    <div class="prize">
        <div class="container">
            <div class="prize-wrapper">
                <div class="prize-texts">
                    <h3 class="prize__title title">Возможность <b> выиграть</b> множество различных <b>призов!</b></h3>
                    <p class="prize__subtitle sub-title">Выполняйте активности в нашем боте или приложении, и зарабатывайте
                        монеты, которые можно потратить на дополнительные ресурсы в виде мегабайт, минут, СМС, а также
                        приобрести товары в нашем маркет-плейсе
                    </p>
                    <app-btn />
                </div>
                <div class="prize__img">
                    <img src="/images/prize-img.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.prize {
    background-image: url('/images/prize-bg.png');
    background-repeat: no-repeat;
    background-position: center;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 75px 0;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 45%;
    }
}
</style>