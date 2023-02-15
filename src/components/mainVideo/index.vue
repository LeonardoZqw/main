<template>
  <!-- 视频部分 -->
  <div class="video">
    <div class="video-box">
      <video autoplay loop>
        <source src="./video/InspurAd.mp4">
      </video>
    </div>
  </div>
</template>

<script>
export default {
  name: 'mainVideo',
}
</script>

<style scoped lang="less">
  .video {
        width: 100%;
        height: 604px;
        background-image: url("./images/ad.png");
        background-repeat: no-repeat;
        display: flex;
        justify-content: center;
        .video-box {
            width: 988.08px;
            height: 604px;
            display: flex;
            align-items: center;
            video {
                width: 988.08px;
                height: 555.75px;
            }
        }
    }
</style>
