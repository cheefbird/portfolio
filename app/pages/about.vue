<template>
  <div>This page is about me!</div>
  <button class="primary" @click="enableCustomLayout">Update layout</button>
</template>

<script setup>
useHead({
  title: 'About Page',
});
function enableCustomLayout() {
  setPageLayout('another');
}
</script>
