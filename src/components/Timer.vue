<script setup>
  const Today = new Date();

  let thisYear = Today.getFullYear();
  let nextYear = Today.getFullYear() + 1;

  // 目標日期
  let countDownTime = new Date("January 01 " + nextYear + " 00:00:00");

  function remainTime() {

    let timeNow = new Date();

    let remain = countDownTime - timeNow;

    let sec = Math.floor(remain/1000)%60;
    let min = Math.floor(remain/1000/60)%60;
    let hour = Math.floor(remain/1000/60/60)%24;
    let day = Math.floor(remain/1000/60/60/24);

    document.getElementById('thisYear').innerHTML = thisYear;
    if (day <= 0) {
      if (hour <= 0) {
        if (min <= 0) {
          if (sec <= 0) {
            var str = thisYear + "已成為過去式，讓我們展望未來，讓" + nextYear + "成為美好的一年。";
            document.getElementById('timer').innerHTML = str;
          } else {
            var str = "餘下" + sec + "秒";
            document.getElementById('timer').innerHTML = str;
          };
        } else {
          var str = "餘下" + min + "分鐘" + sec + "秒。";
          document.getElementById('timer').innerHTML = str;
        };
      } else {
        var str = "餘下" + hour + "小時" + min + "分鐘" + sec + "秒。";
        document.getElementById('timer').innerHTML = str;
      };
    } else {
      var str = "餘下" + day + "天" + hour + "小時" + min + "分鐘" + sec + "秒。";
      document.getElementById('timer').innerHTML = str;
    };
  }

  // 重複呼叫函數 remainTime()
  const timeinterval = setInterval(function(){
    var t = countDownTime - (new Date());

    if(t<0){
      clearInterval(timeinterval);
      // 時間到了
    }else{
      remainTime()
    }
  },1000);
</script>

<template>
  <div class="timer-container">
    <div class="timer-box">
      <div id="thisYear" class="thisYear"></div>
      <div id="timer" class="timer"></div>
    </div>
  </div>
</template>

<style scoped>
  .timer-box {
    text-align: center;
  }

  .thisYear {
    color: #AA3344;
    font-family: 'Hanken Grotesk', sans-serif;
    font-weight: 900;
    font-size: 82px;
    text-shadow: 0 0 24px #BB4455;
  }

  .timer {
    font-size: 36px;
  }

  @media (max-width: 1024px) {
    .timer-container {
      display: flex;
      flex-wrap: wrap;
      justify-items: center;
      justify-content: center;
      padding: 36px 0;
    }
  }

  @media (min-width: 1024px) {
    .timer-container {
      align-content: center;
      display: flex;
      flex-wrap: wrap;
      justify-items: center;
      justify-content: center;
      min-height: 100vh;
    }
  }
</style>
