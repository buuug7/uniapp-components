<template>
  <view>
    <text class="simple-loading-skeleton"></text>
  </view>
</template>

<script>
export default {
  name: "SimpleLoadingSkeleton"
};
</script>

<style>
.simple-loading-skeleton {
  background-color: #eee;
  background-image: linear-gradient(90deg, #eee, #f5f5f5, #eee);
  background-size: 200px 100%;
  background-repeat: no-repeat;
  /*border-radius: 4px;*/
  display: inline-block;
  line-height: 1;
  width: 100%;
  animation: progress 1.2s ease-in-out infinite;
  height: 15px;
}

@keyframes progress {
  0% {
    background-position: -200px, 0;
  }
  100% {
    background-position: calc(200px + 100%), 0;
  }
}
</style>
