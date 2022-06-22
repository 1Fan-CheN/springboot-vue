<template>
  <div>
<!--    头部-->
    <HomeHeader />
<!--    主体-->
    <div style="display: flex">
<!--      侧边栏-->
      <HomeAside />
<!--      主体-->
      <router-view style="flex: 1"/>
    </div>
  </div>
</template>

<style>
</style>

<script>
import HomeHeader from '@/components/HomeHeader'
import HomeAside from '@/components/HomeAside'

export default {
  name: 'HomeLayout',
  components: {
    HomeHeader,
    HomeAside
  }
}
</script>
