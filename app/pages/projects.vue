<template>
  <div>
    <h2 class="text-2xl font-semibold mb-10">Projects</h2>
    <ProjectList />
  </div>
</template>

<script setup>
useHead({
  title: 'Projects',
  htmlAttrs: {
    lang: 'en',
  },
  link: [
    {
      rel: 'icon',
      type: 'image/png',
      href: '/favicon.ico',
    },
  ],
});
</script>
