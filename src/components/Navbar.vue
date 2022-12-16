<script setup>
import { ref, onMounted } from 'vue';
import AppBtn from './AppBtn.vue';

const scrollPosition = ref(null);

const updateScroll = () => {
    scrollPosition.value = window.scrollY
};
onMounted(() => {
    window.addEventListener('scroll', updateScroll);
})
</script>

<template>
    <div :class="['navbar', { 'change__color': scrollPosition > 50 }]">
        <div class="container">
            <div class="navbar-wrapper">
                <div class="navbar__logo">
                    <img src="/images/logo.png" alt="">
                </div>
                <div class="navbar-links">
                    <router-link class="navbar__link" to="#">Главная</router-link>
                    <router-link class="navbar__link" to="#">Преимущества</router-link>
                    <router-link class="navbar__link" to="#">Бот</router-link>
                </div>
                <div class="navbar-wrapper__btn">
                    <app-btn />
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.navbar {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    padding: 15px 0;
    background: transparent;
    z-index: 111;
    transition: all 0.5s;

    &.change__color {
        background-color: #fff;
        box-shadow: 0 0 4px rgb(120 37 141 / 15%);
    }

    &-wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;

        &__link {
            font-weight: 600;
            font-size: 16px;
            line-height: 24px;
            color: #FFFFFF;
        }
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
            color: #FE6101;
        }
    }
}
</style>