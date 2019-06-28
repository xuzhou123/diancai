<template>
  <div class="home">
    <Swipe></Swipe>
    <Tabbar></Tabbar>
  </div>
</template>

<script>
import Swipe from '@/components/common/Swipe.vue'
import Tabbar from '@/components/common/Tabbar.vue'
export default {
  name: 'home',
  components: {
    Swipe,
    Tabbar
  }
}
</script>
