<script setup>
  defineProps({
    url: {
      type: String,
      required: true
    }
  })
</script>

<template>
  <iframe width="560" height="315" v-bind:src="url" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</template>

<style scoped>
  iframe {
    border-radius: 12px;
  }
</style>
