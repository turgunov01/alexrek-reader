<template>
    <div class="blog">
        <div class="blog-container">
            <h1 class="blog-heading">Выберите категорию</h1>
            <ul class="blog-cards">
                <li class="blog-card">
                    <nuxt-link :to="`/lections/`">Лекции</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/`">Материалы</nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts" setup></script>