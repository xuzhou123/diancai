<template>
    <div class="tabbar">

      <mt-tab-container v-model="active" swipeable>
        <mt-tab-container-item id="home1">
          <div style="height:100px;background:#ccc;"></div>
        </mt-tab-container-item>
        <mt-tab-container-item id="play1">
          <div style="height:100px;background:red;"></div>
        </mt-tab-container-item>
        <mt-tab-container-item id="order1">
          <div style="height:100px;background:green;"></div>
        </mt-tab-container-item>
      </mt-tab-container>

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
import { TabContainer, TabContainerItem, Tabbar, TabItem } from 'mint-ui'
export default {
  name: 'Tabbar',
  components: {
    'mt-tab-container': TabContainer,
    'mt-tab-container-item': TabContainerItem,
    'mt-tabbar': Tabbar,
    'mt-tab-item': TabItem
  },
  data () {
    return {
      active: 'home1',
      selected: 'home'
    }
  },
  watch: {
    active (newVal, oldVal) {
      console.log(newVal, oldVal)
    },
    selected (newVal, oldVal) {
      this.active = newVal + '1'
      console.log(newVal, oldVal)
    }
  },
  methods: {
  }
}
</script>

<style scoped>

</style>
