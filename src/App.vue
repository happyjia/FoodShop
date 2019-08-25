<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide   v-if="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuider/FooterGuide'
export default {
  name: 'App',
  components: {FooterGuide}
}
</script>

<style>

</style>
