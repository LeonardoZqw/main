<template>
  <!-- 顶部 -->
  <div class="top">
    <div class="top-bar">
      <div class="top-logo">
        <img src="./images/logo.png" alt="">
      </div>
      <div class="top-time">
        <p>{{nowTime}}</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'mainTop',
    data() {
      return {
        nowTime: ''
      }
    },
    mounted() {
      this.timeNumber()
    },
    methods: {
      // 获取前 xx年xx月xx日 星期x xx:xx
      timeNumber() {
        let today = new Date()
        let nowMonth = this.twoDigits((today.getMonth()+1))
        let nowDate = this.twoDigits(today.getDate())
        let nowHour = this.twoDigits(today.getHours())
        let nowMinute = this.twoDigits(today.getMinutes())
        this.nowTime = today.getFullYear() + '年' + nowMonth + '月' + nowDate + '日' + ' ' + this.getWeekDate() + ' ' + nowHour + ':' + nowMinute
      },
      // 为单位的日期添加0，变为两位
      twoDigits (val) {
        if (val < 10) return '0' + val
        return val
      },
      // 获取当前周几
      getWeekDate(time = new Date()) {
        let weeks = new Array("星期日", "星期一", "星期二", "星期三", "星期四", "星期五", "星期六");
        let date = new Date(time);
        let day = date.getDay();
        return weeks[day];
      }
    }
  }
</script>

<style scoped lang="less">
  .top {
    width: 100%;
    height: 127px;
    line-height: 127px;
    // background-color: rgb(255, 145, 145);
    background-image: url("./images/top.png");
    background-repeat: no-repeat;

    .top-bar {
      width: 1000px;
      margin: 0 auto;
      .top-logo {
        width: 249px;
        height: 127px;
        float: left; // 向左浮动
        display: flex;
        align-items: center;
        img {
          margin: 0 auto;
        }
      }
      .top-time {
        // height: 127px;  用于WebStorm
        float: right; // 向右浮动
        p {
          // position: relative;
          // left: 0;
          // top: -35px;  以上3行用于WebStorm
          font-size: 35px;
          font-weight: bold;
          color: white;
        }
      }
    }
  }
</style>
