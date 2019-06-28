<template>
    <div class="tabbar">
      <mt-tabbar  v-model="selected">
        <mt-tab-item id="home">
          <img slot="icon" src="../../assets/common/home.png" alt="">
          首页
        </mt-tab-item>
        <mt-tab-item id="play">
          <img slot="icon" src="../../assets/common/order.png" alt="">
          娱乐
        </mt-tab-item>
        <mt-tab-item id="order">
          <img slot="icon" src="../../assets/common/index.png" alt="">
          订单
        </mt-tab-item>
        <mt-tab-item id="index">
          <img slot="icon" src="../../assets/common/index.png" alt="">
          我的
        </mt-tab-item>
      </mt-tabbar>
    </div>
</template>

<script>
import { Tabbar, TabItem } from 'mint-ui'
export default {
  name: 'Tabbar',
  components: {
    'mt-tabbar': Tabbar,
    'mt-tab-item': TabItem
  },
  data () {
    return {
      selected: 'home'
    }
  },
  watch: {
    selected (newVal, oldVal) {
      console.log(newVal, oldVal)
    }
  },
  methods: {
  }
}
</script>

<style scoped>

</style>
