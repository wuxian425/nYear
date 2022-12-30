<script setup>
  defineProps({
    title: {
      type: String,
      required: true
    },
    content: {
      type: String,
      required: true
    },
    live: {
      type: String,
      required: true
    }
  })
</script>

<template>
  <div class="card">
    <h1 class="t-color">{{ title }}</h1>
    <p>{{ content }}</p>
    <a v-bind:href="live">前往直播</a>
  </div>
</template>

<style scoped>
.card {
  background-color: #FAFAFA;
  margin: 8px 0;
  padding: 16px;
}

h1 {
  font-size: 24px;
}

p {
  font-size: 16px;
  margin-bottom: 12px;
}

a {
  border: 1px solid #AA3344;
  cursor: pointer;
  display: inline-block;
  padding: 2px 6px;
}

a:hover {
  padding: 2px 12px;
}
</style>
