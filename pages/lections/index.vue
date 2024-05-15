<template>
    <div class="blog">
        <div class="blog-container">
            <h1 class="blog-heading">Лекции</h1>
            <ul class="blog-cards">
                <li class="blog-card">
                    <nuxt-link :to="`/lections/2024`">2024</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/lections/2023`">2023</nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts" setup></script>