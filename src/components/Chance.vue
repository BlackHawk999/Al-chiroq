<script setup>
import AppBtn from './AppBtn.vue'

</script>

<template>
    <div class="chance">
        <div class="container">
            <div class="chance-wrapper">
                <div class="chance__img">
                    <img src="/images/chance-img.png" alt="">
                </div>
                <div class="chance-texts">
                    <h3 class="chance__title title"><b>6 Шансов</b> получения бонуса</h3>
                    <p class="chance__subtitle sub-title">Заходите в приложение Al Chiroq в разделе “Купить шансы” вы сможете
                        приобрести дополнительные шансы для получения бонусов. Они доступны по выгодным ценам, покупайте
                        и выигрывайте призы!
                    </p>
                    <app-btn />
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.chance {
    padding: 35px 0 100px 0;
    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    &-texts {
        display: flex;
        flex-direction: column;
        width: 42%;
    }

}
</style>