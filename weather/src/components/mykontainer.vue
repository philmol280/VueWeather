<template>
  <div class="informer-container">
     <temperature :tempReal=tempReal :tempFeel=tempFeel>
      </temperature>

      <div class="flex-break"></div>

      <humidity :humid=humid></humidity>

      <div class="vertical-divider"></div>
      <wind :windSpeed=windSpeed></wind>
  </div>
</template>

<script>
import humidity from './humidity.vue'
import wind from './wind.vue'
import temperature from './temperature.vue'
export default {

  name: 'mykontainer',
  components: {
    humidity,
    wind,
    temperature
  },
  props: {
    tempReal: String,
    tempFeel: String,
    humid: String,
    windSpeed: String
  }
}
</script>

<style>
.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  min-height: 255px;
  padding: 30px;
  background-image: url('img/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
.flex-break{
  flex-basis: 100%;
  height: 0;
}
.vertical-divider{
  height: 70px;
  width: 1px;
  background-color: #fff;
  vertical-align: middle;
  display: table-cell;
}
</style>