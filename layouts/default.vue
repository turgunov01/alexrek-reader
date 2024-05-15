<script lang="ts" setup>
import { useRouter } from 'vue-router';
const $router = useRouter()
</script>

<template>
    <div class="wrapper">
        <div class="container">
            <nav class="nav">
                <div class="nav-container">
                    <p class="nav-logo">Logo</p>
                    <p class="nav-social">Social media</p>
                </div>
            </nav>
            <slot />
            <div class="footer">
                <div class="container">
                    <div class="footer-buttons">
                        <button class="footer-button" @click="$router.back()">Назад</button>
                        <nuxt-link to="/" class="footer-button">Домой</nuxt-link>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.container {
    display: flex;
    flex-direction: column;
    row-gap: 2rem;
}
</style>
