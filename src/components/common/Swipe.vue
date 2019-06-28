<template>
    <div class="swipe">
      <mt-swipe :auto="4000">
        <mt-swipe-item><img src="../../assets/swipe/swipe1.jpg" alt=""></mt-swipe-item>
        <mt-swipe-item><img src="../../assets/swipe/swipe2.jpg" alt=""></mt-swipe-item>
        <mt-swipe-item><img src="../../assets/swipe/swipe3.jpg" alt=""></mt-swipe-item>
        <mt-swipe-item><img src="../../assets/swipe/swipe4.jpg" alt=""></mt-swipe-item>
      </mt-swipe>
    </div>
</template>

<script>
import { Swipe, SwipeItem } from 'mint-ui'
export default {
  name: 'Swipe',
  components: {
    'mt-swipe': Swipe,
    'mt-swipe-item': SwipeItem
  }
}
</script>

<style scoped lang="scss">
.swipe {
  height: 150px;
  img {
    height: 150px;
    width: 100%;
  }
}
</style>
