<template>
    <div class="blog">
        <div class="blog-container">
            <h1 class="blog-heading">Материалы - {{ year }} </h1>
            <ul class="blog-cards">
                <li class="blog-card">
                    <nuxt-link :to="`/materials/${year}/1`">Материалы 1</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/${year}/2`">Материалы 2</nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts" setup>

import { useRouter } from 'vue-router';
const $router = useRouter()

const year = $router.currentRoute.value.params.id

</script>

<style lang="scss" scoped></style>