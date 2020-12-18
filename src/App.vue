<template>
  <div id='app'>
    <v-header></v-header>
  </div>
</template>

<script>

import vHeader from './components/v-header/v-header'

export default {
  name: 'app',
  components: {
    vHeader
  }
}
</script>
<style lang="stylus">
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
</style>
