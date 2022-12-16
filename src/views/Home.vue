<script setup>
import Navbar from '../components/Navbar.vue'
import Intro from '../components/Intro.vue';
import TelegramBot from '../components/TelegramBot.vue';
import Premium from '../components/Premium.vue'
import Bonus from '../components/Bonus.vue';
import Prizes from '../components/Prizes.vue';
import Chance from '../components/Chance.vue';
import AppFooter from '../components/AppFooter.vue';

</script>

<template>
    <div class="home-page">
        <navbar />
        <intro />
        <telegram-bot />
        <premium />
        <bonus />
        <prizes />
        <chance />
        <app-footer />
    </div>
</template>


<style>

</style>