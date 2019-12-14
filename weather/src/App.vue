<template>
  <div id="app">
    <div class="informer-container">
      <div class="temperature">
        <img src="img/thermometer.png">
        <div class="temp-real">1</div>
        <div class="temp-feel">-3.8</div>
      </div>
      <div class="flex-break"></div>
      <div class="humidity">
        <img src="img/humidity.png"> 12 <small>%</small>
      </div>
      <div class="vertical-divider"></div>
      <div class="wind">
        <img src="img/wind.png"> 12 <small>м/с</small>
      </div>
    </div>
  </div>
</template>

<script>
import mykontainer from './components/mykontainer.vue'
import humidity from './components/humidity.vue'
import wind from './components/wind.vue'
import temperature from './components/temperature.vue'
export default {
  name: 'app',
  components: {
    mykontainer,
    humidity,
    wind,
    temperature
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
