<script setup>
  import Player from '../components/Player.vue';

  this.$router.push({
    path: '/live',
    query: {
      url: url
    }
  });
</script>

<template>
  <div class="live-container">
    <Player 
      :url="this.$route.query.url"
      id="Player"
    />
  </div>
</template>

<style scoped>
  .live-container {
    padding-top: 32px;
  }
</style>