<template>
  <div class="about">
    <div>
      <h3>這裏是一個整理跨年資訊的站點。</h3>
      <br>

      <p>本質上是我在 2021 年底製作的 Scratch 項目「嗨跨年！」使用 Vue.js 的重置版，旨在讓用戶在跨年時能快速找到自己想看的節目。</p>
      <br>
      
      <footer>(c) 2022 BobYang. 本項目在 <a href="https://github.com/wuxian425/nYear">Github</a> 上開放源始碼。</footer>
    </div>
  </div>
</template>

<style>
  footer {
    color: #bbb;
    font-size: 12px;
  }

  .about {
    display: flex;
    padding: 32px;
    justify-items: center;
    justify-content: center;
  }

  @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-items: center;
      justify-content: center;
    }
  }
</style>
