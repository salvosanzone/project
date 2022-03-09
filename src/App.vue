<template>

  <div>
    <MyHeader />
    <MyMain />
  </div>
  
</template>

<script>
// import axios from 'axios'
import MyHeader from './partials/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import "@fontsource/quicksand";

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,

  },
  
}
</script>

<style lang="scss">
@import './assets/style/general.scss';

</style>
