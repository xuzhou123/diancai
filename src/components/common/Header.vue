<template>
  <div class="header">
    <mt-header title="标题过长会隐藏后面的内容啊哈哈哈哈">
      <mt-button icon="back" slot="left">返回</mt-button>
      <mt-button icon="more" slot="right"></mt-button>
    </mt-header>
  </div>
</template>

<script>
import { Header, Button } from 'mint-ui'
export default {
  name: 'Header',
  components: {
    'mt-header': Header,
    'mt-button': Button
  }
}
</script>

<style scoped>

</style>
