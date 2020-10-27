<template>
  <div class="basic text-center" @click="buttonClick">
    <div class="row justify-content-center">
      <div class="col-6">{{ current }}</div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info">+</button>
        <button class="btn btn-info">-</button>
        <button class="btn btn-info">x</button>
        <button class="btn btn-info">/</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info btn-lg">7</button>
        <button class="btn btn-info btn-lg">8</button>
        <button class="btn btn-info btn-lg">9</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info btn-lg">4</button>
        <button class="btn btn-info btn-lg">5</button>
        <button class="btn btn-info btn-lg">6</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info btn-lg">1</button>
        <button class="btn btn-info btn-lg">2</button>
        <button class="btn btn-info btn-lg">3</button>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-6">
        <button class="btn btn-info btn-md">0</button>
        <button class="btn btn-info btn-md">.</button>
        <button class="btn btn-info btn-md">C</button>
        <button class="btn btn-info btn-md">=</button>
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
  methods: {
    buttonClick: function (e) {
      let value = e.target.innerText;

      this.$emit("addNumber", value);
    },
  },
  components: {},
};
</script>


<style scoped>
</style>