<template>
  <div id="wrapper">
    <mainTop></mainTop>
    <mainVideo></mainVideo>
<!--    <menuHome></menuHome>-->
<!--    <selectCards></selectCards>-->
<!--    <selectBusinessReg></selectBusinessReg>-->
<!--    <selectBusinessPrint></selectBusinessPrint>-->
    <selectBusinessFiling></selectBusinessFiling>
  </div>
</template>

<script>
// 引入非路由组件
import mainTop from './components/mainTop'
import mainVideo from './components/mainVideo'

// 引入路由组件
// import menuHome from './pages/menuHome'
// import selectCards from './pages/selectCards'
// import selectBusinessReg from './pages/selectBusinessReg'
// import selectBusinessPrint from './pages/selectBusinessPrint'
import selectBusinessFiling from './pages/selectBusinessFiling'

export default {
  name: 'App',
  components: {
    mainTop,
    mainVideo,
    // menuHome,
    // selectCards,
    // selectBusinessReg,
    // selectBusinessPrint,
    selectBusinessFiling
  }
}
</script>

<style>
  #wrapper {
    width: 1080px;
    height: 1920px;
  }
</style>
