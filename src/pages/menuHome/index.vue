<template>
  <!-- 菜单部分 -->
  <div class="menu-list">
    <div class="main4">
      <img src="./images/main4.png" alt="">
    </div>
    <div class="top-menu">
      <div class="orderReg">
        <img src="./images/meau_button/预约-挂号.png" alt="">
      </div>
      <div class="payFees">
        <img src="./images/meau_button/缴费.png" alt="">
      </div>
      <div class="recharge">
        <img src="./images/meau_button/充值.png" alt="">
      </div>
      <div class="selfPrint">
        <img src="./images/meau_button/自助打印.png" alt="">
      </div>
    </div>
    <div class="bottom-menu">
      <div class="filing">
        <img src="./images/meau_button/建档.png" alt="">
      </div>
      <div class="mzSearch">
        <img src="./images/meau_button/门诊查询.png" alt="">
      </div>
      <div class="zySearch">
        <img src="./images/meau_button/住院查询.png" alt="">
      </div>
      <div class="zyRecharge">
        <img src="./images/meau_button/住院充值.png" alt="">
      </div>
      <div class="more">
        <img src="./images/meau_button/更多.png" alt="">
      </div>
    </div>
    <div class="bottom-info">
      <div class="terminal-location">
        <img src="./images/位置.png" alt="">
        <p>终端位置:{{currentPosition}}</p>
      </div>
      <div class="terminal-number">
        <p>终端号:{{terminalNumber}}</p>
        <img src="./images/设备编号.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'menuHome',
    data() {
      return {
        currentPosition: '涉县医院',
        terminalNumber: 'LC001'
      }
    },
    methods: {

    }
  }
</script>

<style scoped lang="less">
  .menu-list {
    // display: none;
    width: 100%;
    height: 1189px;
    background-image: url("./images/body.png");
    background-repeat: no-repeat;
    // 主菜单白色背景
    .main4 {
      position: relative;
      top: 0px;
      left: 19px;
    }
    // 预约挂号--自助打印
    .top-menu {
      position: relative;
      left: 74px;
      top: -1020px;
      .orderReg {

      }
      .payFees {
        position: relative;
        left: 480px;
        top: -492px;
      }
      .recharge {
        position: relative;
        left: 480px;
        top: -470px;
      }
      .selfPrint {
        position: relative;
        left: 0px;
        top: -450px;
      }
    }
    // 建档--更多
    .bottom-menu {
      position: relative;
      top: -1400px;
      left: 70px;
      height: 135px;
      // width: ;
      // background-color: chartreuse;
      display: block;
      div {
        float: left;
        margin: 0 42px;
        // background-color: cornflowerblue;
      }
      /* .filing {

      }
      .mzSearch {

      }
      .zySearch {

      }
      .zyRecharge {

      }
      .more {

      } */
    }
    // 终端位置和终端号
    .bottom-info {
      height: 67px;
      width: 980px;
      position: relative;
      left: 0;
      top: -1350px;
      margin: 0 auto;
      .terminal-location {
        float: left;
        height: 67px;
        width: 60%;
      }
      .terminal-number {
        float: right;
        height: 67px;
        width: 40%;
        p {
          float: right;
        }
        img {
          float: right;
        }
      }
      img {
        float: left;
      }
      p {
        float: left;
        line-height: 67px;
        color: white;
        font-size: 28px;
        font-family: 黑体;
        font-weight: bolder;
      }
    }
  }
</style>
