<template>
  <div>
    <el-menu
      style="width: 200px; height: calc(100vh - 50px)"
      active-text-color="#ffd04b"
      background-color="#545c64"
      class="el-menu-vertical-demo"
      default-active="1"
      text-color="#fff"
      @open="handleOpen"
      @close="handleClose"
    >
      <el-sub-menu index="1">
        <template #title>
          <el-icon><location /></el-icon>
          <span>Navigator One</span>
        </template>
        <el-menu-item index="1-1">item one</el-menu-item>
        <el-menu-item index="1-2">item one</el-menu-item>
        <el-menu-item index="1-3">item three</el-menu-item>
        <el-sub-menu index="1-4">
          <template #title>item four</template>
          <el-menu-item index="1-4-1">item one</el-menu-item>
        </el-sub-menu>
      </el-sub-menu>
      <el-menu-item index="2">
        <el-icon><icon-menu /></el-icon>
        <span>Navigator Two</span>
      </el-menu-item>
      <el-menu-item index="3">
        <el-icon><setting /></el-icon>
        <span>Navigator Three</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script setup>
import {
  Menu as IconMenu,
  // eslint-disable-next-line no-unused-vars
  Location,
  Setting
} from '@element-plus/icons-vue'

const handleOpen = (key, keyPath) => {
  console.log(key, keyPath)
}
const handleClose = (key, keyPath) => {
  console.log(key, keyPath)
}
</script>

<script>
export default {
  name: 'HomeAside'
}
</script>

<style scoped>

</style>
