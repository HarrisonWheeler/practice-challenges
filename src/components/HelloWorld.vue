<template>
  <div class="hello container-fluid">
    <div class="row justify-content-center">
      <div class="col-6">Result:</div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">+</button>
        <button class="btn btn-info">-</button>
        <button class="btn btn-info">X</button>
        <button class="btn btn-info">÷</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">7</button>
        <button class="btn btn-info">8</button>
        <button class="btn btn-info">9</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">4</button>
        <button class="btn btn-info">5</button>
        <button class="btn btn-info">6</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">1</button>
        <button class="btn btn-info">2</button>
        <button class="btn btn-info">3</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">0</button>
        <button class="btn btn-info">.</button>
        <button class="btn btn-info">C</button>
        <button class="btn btn-info">=</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "calculator",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
