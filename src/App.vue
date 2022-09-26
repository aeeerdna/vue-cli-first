<template>
  <div id="app">
    <p>{{ saluto }}</p>
    <div v-for="(item, index) in test" :key="index">
      {{ item }}
      <FirstComponent />
    </div>
  </div>
</template>

<script>
import FirstComponent from "./components/first-component.vue";

export default {
  name: "App",
  data() {
    return {
      saluto: "Hi to everybody",
      test: [1, 3, 6, 9, 12, 1],
    };
  },
  components: {
    FirstComponent,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
