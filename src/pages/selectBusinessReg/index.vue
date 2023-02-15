<template>
  <!-- 选择办理的业务-->
  <div class="wrapper">
    <div class="main1">
      <img src="./images/main1.png" alt="">
    </div>
    <div class="select-business">
      <div class="text">
        <p>请选择办理的业务</p>
      </div>
      <div class="business-menu">
        <div class="same-dayReg">
          <img src="./images/button/当日挂号.png" alt="">
        </div>
        <div class="regOrder">
          <img src="./images/button/预约挂号.png" alt="">
        </div>
        <div class="numOrder">
          <img src="./images/button/预约取号.png" alt="">
        </div>
        <div class="smartDiagnose">
          <img src="./images/button/智能导诊.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'selectBusiness',
  }
</script>

<style scoped lang="less">
  .wrapper {
    width: 1080px;
    height: 1189px;
    background-image: url("./images/body.png");
    background-repeat: no-repeat;
    .main1 {
      position: relative;
      left: 20px;
      width: 1039px;
      height: 1021px;

    }
    .select-business {
      width: 868px;
      height: 600px;
      position: relative;
      left: 106px;
      top: -830px;
      .text {
        width: 868px;
        text-align: center;
        margin-bottom: 165px;
        color: rgb(0, 116, 233);
        font-size: 48px;
        font-weight: bold;
        font-family: 黑体;
      }
      .business-menu {
        width: 912px;
        height: 635px;
        div {
          float: left;
          margin: 13px 10px;
        }
      }
    }
  }
</style>
