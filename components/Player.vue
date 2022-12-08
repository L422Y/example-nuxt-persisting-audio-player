<template>
  <div id="player">
    (persistent audio player alive for: <span v-if="tick">{{ tick }}s)</span>
    <audio controls autoplay src="/nyte_-_pleasure.mp3"></audio>
  </div>
</template>
<script setup>
let tick = ref(1);
let tickTimer = setInterval(() => {
  tick.value++;
}, 1000);
</script>
<script>
export default {
  unmounted() {
    // clearInterval(this.tickTimer)
  },
};
</script>
