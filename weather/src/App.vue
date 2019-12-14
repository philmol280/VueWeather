<template>
  <div id="app">
    <mykontainer tempReal="1" tempFeel="-3.8" humid="12" windSpeed="12npm "></mykontainer>
  </div>
</template>

<script>
import mykontainer from './components/mykontainer.vue'
export default {
  name: 'app',
  components: {
    mykontainer
  }
}
</script>

<style>
#app {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: rgb(244, 123, 186);
  background: linear-gradient(-25deg, rgba(244, 123, 186, 0.5) 20%, rgba(90, 95, 245, 0.5) 80%);
}
</style>
