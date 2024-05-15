<template>
  <div class="blog">
    <div class="blog-container">
      <h1 class="blog-heading routing">
        <span>
          <nuxt-link to="/materials/">Материалы</nuxt-link>
          <span class="blog-heading-bread">/</span>
          <nuxt-link :to="`/materials/${Route.key}`"> {{ Route.key }}</nuxt-link>
          <span class="blog-heading-bread">/</span>
          <p class="blog-heading-link"> {{ Route.id }} </p>
        </span>
      </h1>
      <div class="blog-html" v-html="Route.html"></div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { useRouter } from 'vue-router';
import { ref } from 'vue';
const $router = useRouter()

const Route = ref({
  key: "",
  id: $router.currentRoute.value.params.id,
  html: `<div style="width: 540px; height: 682px; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 16px; display: inline-flex">
  <div style="align-self: stretch"><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I'm a passionate, </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">self-proclaimed designer</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word"> who specializes in full stack development (React.js & Node.js). I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User experience, pixel perfect design, and writing clear, readable, highly performant code matters to me.</span></div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I began my journey as a web developer in 2015, and since then, I've continued to grow and evolve as a developer, taking on new challenges and learning the latest technologies along the way. Now, in my early thirties, 7 years after starting my web development journey, I'm building cutting-edge web applications using modern technologies such as Next.js, TypeScript, Nestjs, Tailwindcss, Supabase and much more.</div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I am very much a progressive thinker and enjoy working on products end to end, from ideation all the way to development.</div>
  <div style="align-self: stretch"><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">When I'm not in full-on developer mode, you can find me hovering around on twitter or on indie hacker, witnessing the journey of early startups or enjoying some free time. You can follow me on </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">Twitter</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word"> where I share tech-related bites and build in public, or you can follow me on </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">GitHub</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">.</span></div>
  <div style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Finally, some quick bits about me.</div>
  <div style="align-self: stretch; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
    <div style="flex: 1 1 0; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">B.E. in Computer Engineering</div>
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Full time freelancer</div>
    </div>
    <div style="flex: 1 1 0; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Avid learner</div>
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Aspiring indie hacker</div>
    </div>
  </div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">One last thing, I'm available for freelance work, so feel free to reach out and say hello! I promise I don't bite 😉</div>
</div><div style="width: 540px; height: 682px; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 16px; display: inline-flex">
  <div style="align-self: stretch"><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I'm a passionate, </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">self-proclaimed designer</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word"> who specializes in full stack development (React.js & Node.js). I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User experience, pixel perfect design, and writing clear, readable, highly performant code matters to me.</span></div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I began my journey as a web developer in 2015, and since then, I've continued to grow and evolve as a developer, taking on new challenges and learning the latest technologies along the way. Now, in my early thirties, 7 years after starting my web development journey, I'm building cutting-edge web applications using modern technologies such as Next.js, TypeScript, Nestjs, Tailwindcss, Supabase and much more.</div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">I am very much a progressive thinker and enjoy working on products end to end, from ideation all the way to development.</div>
  <div style="align-self: stretch"><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">When I'm not in full-on developer mode, you can find me hovering around on twitter or on indie hacker, witnessing the journey of early startups or enjoying some free time. You can follow me on </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">Twitter</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word"> where I share tech-related bites and build in public, or you can follow me on </span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; text-decoration: underline; line-height: 24px; word-wrap: break-word">GitHub</span><span style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">.</span></div>
  <div style="color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Finally, some quick bits about me.</div>
  <div style="align-self: stretch; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
    <div style="flex: 1 1 0; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">B.E. in Computer Engineering</div>
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Full time freelancer</div>
    </div>
    <div style="flex: 1 1 0; flex-direction: column; justify-content: flex-start; align-items: flex-start; gap: 10px; display: inline-flex">
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Avid learner</div>
      <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">Aspiring indie hacker</div>
    </div>
  </div>
  <div style="align-self: stretch; color: white; font-size: 16px; font-family: Inter; font-weight: 400; line-height: 24px; word-wrap: break-word">One last thing, I'm available for freelance work, so feel free to reach out and say hello! I promise I don't bite 😉</div>
</div>`,
  path: $router.currentRoute.value.path,
})

const categories = ['matematika', 'khimiya', 'istoriya', 'algebra', 'geometriya']

categories.forEach((category) => {
  if (Route.value.path.includes(category)) {
    Route.value.key = category
  }
})

</script>

<style lang="scss" scoped>
.blog {
  height: 100%;
  max-height: 83vh;
  overflow: auto;
  background: linear-gradient(180deg, rgba(255, 255, 255, 0.2) 40%, #1F2937 100%);
  position: relative;
}
</style>