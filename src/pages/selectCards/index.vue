<template>
  <!-- 选择就诊介质 -->
  <div class="wrapper">
    <div class="main5">
      <img src="./images/main5.png" alt="">
    </div>
    <div class="select-card">
      <div class="text">
        <p>请选择就诊介质</p>
      </div>
      <div class="card-menu">
        <div class="patientCard">
          <img src="./images/cards/就诊卡.png" alt="">
        </div>
        <div class="IDCard">
          <img src="./images/cards/身份证.png" alt="">
        </div>
        <div class="patientNumber">
          <img src="./images/cards/门诊号条码.png" alt="">
        </div>
        <div class="healthCard">
          <img src="./images/cards/电子健康卡.png" alt="">
        </div>
        <div class="soc-secCard">
          <img src="./images/cards/社保卡.png" alt="">
        </div>
        <div class="ele-healthCard">
          <img src="./images/cards/电子医保凭证.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'selectCards',
  }
</script>

<style scoped lang="less">
  .wrapper {
    /*position: relative;*/
    /*top: -25px;*/
    width: 1080px;
    height: 1189px;
    background-image: url("./images/body.png");
    background-repeat: no-repeat;
    .main5 {
      position: relative;
      /*top: -24px;*/
      left: 20px;
      width: 1039px;
      height: 1021px;
    }
    .select-card {
      position: relative;
      left: 84px;
      top: -830px;
      .text {
        width: 912px;
        text-align: center;
        margin-bottom: 20px;
        color: rgb(0, 116, 233);
        font-size: 48px;
        font-weight: bold;
        font-family: 黑体;
      }
      .card-menu {
        width: 912px;
        height: 635px;
        div {
          float: left;
          margin: 15px 10px;
        }
      }
    }
  }
</style>
