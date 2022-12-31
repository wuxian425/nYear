<script setup>
  defineProps({
    title: {
      type: String,
      required: true
    },
    hosts: {
      type: String,
      default: "未知"
    },
    cases: {
      type: String,
      default: "未知"
    },
    live: {
      type: String,
      default: "#未知"
    }
  });
</script>

<template>
  <div class="card">
    <h1 class="t-color">{{ title }}</h1>
    <p>主持人：{{ hosts }}</p>
    <p>跨年卡司：{{ cases }}</p>
    <a v-bind:href="live" target="_blank">前往直播</a>
  </div>
</template>

<style scoped>
.card {
  background-color: #FAFAFA;
  margin: 8px 0;
  padding: 16px;
}

h1 {
  display: inline-block;
  font-size: 24px;
  margin-bottom: 16px;
  position: relative;
}

h1:after {
  background-color: #AA334420;
  border-radius: 12px;
  box-shadow: 0 0 8px #AA334420;
  content: '';
  position: absolute;
  z-index: 1;

  top: 60%;
  bottom: 2px;
  left: 10px;
  right: -10px;
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

a:after {
  background-color: transparent;
}
</style>
