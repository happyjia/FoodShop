<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide   v-if="$route.meta.showFooter"/>
  </div>
</template>

<script>
import {mapActions} from 'vuex'
import FooterGuide from './components/FooterGuider/FooterGuide'
export default {
  name: 'App',
  mounted () {
    // this.$store.dispatch('getAddress')
    this.getAddress()
  },
  methods: {
    ...mapActions(['getAddress'])
  },
  components: {FooterGuide}
}
</script>

<style>

</style>
