<template>
  <div class="basic container-fluid text-center" @click="buttonClick">
    <div class="row justify-content-center pt-5">
      <div class="col-6">{{ current }}</div>
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
  name: "basic",
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: {},
};
</script>


<style scoped>
</style>