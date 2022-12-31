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
  font-family: consolas, 'Shippori Mincho', monospace;
  font-weight: 800;
  font-size: 2.6rem;
}

h3 {
  font-size: 1.2rem;
}

.t-color {
  display: block;
  position: relative;
  text-shadow: 0 0 8px #AA3344CC;
}

@media (min-width: 1024px) {
  .t-color {
    display: inline-block;
    top: -8px;
  }

  .t-color:before {
    background-color: #AA334444;
    border-radius: 999px;
    box-shadow: 0 0 8px #AA334422;
    color: #AA334466;
    content: '';
    padding: 25px;
    position: absolute;
    z-index: -1;

    width: 100px;
    height: 100px;

    top: -32px;
    left: -12px;
  }

  .t-color:after {
    background-color: #AA334411;
    color: #AA334466;
    content: '新年快樂';
    font-size: 24px;
    line-height: 0.8;
    padding: 0 8px;
    position: absolute;
    text-shadow: none;
    z-index: -1;

    bottom: -2px;
    right: -32px;
  }
}

/* 手機端 */
.greetings h1,
.greetings h3 {
  margin-left: auto;
  margin-right: auto;
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    margin-left: 0;
    margin-right: 0;
  }
}
</style>
