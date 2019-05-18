<template>
  <el-menu
    :default-active="activeIndex"
    class="el-menu-demo"
    mode="horizontal"
    @select="handleSelect"
    background-color="gray"
    text-color="white"
    active-text-color="#ffd04b"
    style="height: 60px;"
  >
    <el-menu-item index="1">处理中心</el-menu-item>
    <el-menu-item index="2">消息中心</el-menu-item>
    <el-menu-item index="3">订单管理</el-menu-item>
  </el-menu>
</template>

<script>
  export default {
    data () {
      return {
        activeIndex: '1',
      }
    },
    methods: {
      handleSelect (key, keyPath) {
        console.log(key, keyPath)
      }
    }
  }
</script>
