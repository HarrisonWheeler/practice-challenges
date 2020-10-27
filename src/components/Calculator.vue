<template>
  <div class="calculator container-fluid bg-dark full-height">
    <div class="row text-light justify-content-center pt-5">
      <input type="text" class="text-right" v-model="current" />
    </div>
    <div class="buttons">
      <Basic v-bind:current="current" @addNumber="doMath($event)" />
    </div>
  </div>
</template>


<script>
import Basic from "./Basic";
export default {
  name: "calculator",
  data() {
    return {
      current: 0,
    };
  },
  computed: {},
  methods: {
    doMath: function (data) {
      let temp;

      if (Number(data) || data == 0) {
        temp = data;
        if (this.current === 0) this.current = "";
        this.current += "" + temp;
      }
      if (!Number(data)) {
        switch (data) {
          case "/": {
            this.divide();
            break;
          }
          case "C": {
            this.clear();
            break;
          }
          case "x": {
            this.multiply();
            break;
          }
          case "-": {
            this.minus();
            break;
          }
          case "+": {
            this.plus();
            break;
          }
          case "=": {
            this.equals();
            break;
          }
        }
      }
    },
    clear: function () {
      this.current = 0;
    },
    multiply: function () {
      this.current += "*";
    },
    divide: function () {
      this.current += "/";
    },
    plus: function () {
      this.current += "+";
    },
    minus: function () {
      this.current += "-";
    },
    equals: function () {
      this.current = eval(this.current);
    },
  },
  components: {
    Basic,
  },
};
</script>


<style scoped>
.full-height {
  min-height: 100rem;
}
</style>