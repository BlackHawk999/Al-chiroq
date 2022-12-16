<script setup>
import AppLinks from './AppLinks.vue';

</script>

<template>
    <div class="footer">
        <div class="container">
            <div class="footer-wrapper">
                <div class="footer__logo">
                    <img src="/images/footer-logo.png" alt="">
                </div>
                <div class="footer-links">
                    <router-link class="footer__link">Главная</router-link>
                    <router- class="footer__link">Преимущества</router->
                    <router-link class="footer__link">Бот</router-link>
                </div>
                <div class="footer-apps">
                    <app-links />
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss">
.footer {
    background-image: url('/images/footer-bg.png');
    background-color: #FD9A20;

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 40px 0;
    }

    &-links {
        display: flex;
        align-items: center;
    }

    &__link {
        font-weight: 500;
        font-size: 16px;
        line-height: 20px;
        color: #333333;
        transition: all 0.3s;
        cursor: pointer;

        &:not(:last-child) {
            margin-right: 40px;
        }

        &:hover {
            transform: scale(1.05);
            color: #fff;
        }
    }
}
</style>