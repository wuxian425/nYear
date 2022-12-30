<template>
  <div class="greetings">
    <h1 class="t-color">nYear</h1>
    <h3>
      當新的一年將至，何必出外受寒，宅在家跨年豈不美哉？<br>
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 800;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

/* 手機端 */
.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
