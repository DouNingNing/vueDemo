<template>
  <div id="app">
    <m-header></m-header>
    <tab></tab>
    <keep-alive><!--keep-alive可以把dom缓存在内存中，不会重新请求数据-->
      <router-view></router-view>
    </keep-alive>
  </div>
</template>

<script type="text/ecmascript-6">
  import MHeader from 'components/m-header/m-header'
  import Tab from 'components/tab/tab'

  export default {
    components: {
      MHeader,
      Tab
    }
  }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
</style>