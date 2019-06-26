<template>
  <div class="home">
    <Header></Header>
    <Tabbar></Tabbar>
  </div>
</template>

<script>
import Header from '@/components/common/Header.vue'
import Tabbar from '@/components/common/Tabbar.vue'
export default {
  name: 'home',
  components: {
    Header,
    Tabbar
  }
}
</script>
