<template>
  <div>
    This is the music page <span v-if="slug">({{ slug }})</span>
  </div>
  <p>The music player will persist across all /music/ pages and URLs</p>
</template>
<script setup>
let { slug } = useRoute().params;

definePageMeta({
  layout: 'music',
});
</script>
