<template>
  <div class="container mx-auto max-w-2xl">
    <header class="flex justify-between items-center mt-5">
      <div class="flex items-center space-x-12">
        <div>
          <NuxtLink to="/" class="text-xl font-semibold p-2 hover:bg-gray-200">
            Francis B
          </NuxtLink>
        </div>
        <Menu />
      </div>
      <ClientOnly>
        <ColorModeSelector />
      </ClientOnly>
    </header>
    <main class="p-2 mt-10">
      <slot />
    </main>
  </div>
</template>

<script setup>
  useHead({
    titleTemplate: '%s - FB Portfolio',
    link: [
      {
        rel: 'preconnect',
        href: 'https://fonts.googleapis.com',
      },
      {
        rel: 'stylesheet',
        href: 'https://fonts.googleapis.com/css2?family=Fira+Mono&family=Fira+Sans&display=swap',
        crossorigin: '',
      },
    ],
  });
</script>

<style>
  body {
    font-family: 'Fira Sans';
  }
  .fira-mono {
    font-family: 'Fira Mono', monospace;
    font-weight: 400;
    font-style: normal;
  }

  body {
    @apply bg-white dark:bg-gray-900 text-gray-700 dark:text-gray-300;
  }
</style>
