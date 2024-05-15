<template>
    <div class="blog">
        <div class="blog-container">
            <h1 class="blog-heading">Материалы</h1>
            <ul class="blog-cards">
                <li class="blog-card">
                    <nuxt-link :to="`/materials/matematika`">Математика</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/istoriya`">История</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/khimiya`">Химия</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/algebra`">Алгебра</nuxt-link>
                </li>
                <li class="blog-card">
                    <nuxt-link :to="`/materials/geometriya`">Геометрия</nuxt-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts" setup></script>