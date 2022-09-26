<template>
  <div class="red" @click="saluta">Primo vue component</div>
</template>

<script>
export default {
  name: "FirstComponent",
  methods: {
    saluta() {
      console.log("saluta il tuo amico");
    },
  },
};
</script>

<style scoped>
.red {
  background-color: red;
}
</style>
