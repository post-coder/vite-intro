<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },

  methods: {
    count() {
      this.counter++;
    },
  },
};
</script>

<template>
  <button @click="count()">
    Hai premuto questo pulsante {{ counter }} volte
  </button>
</template>

<style scoped>
* {
  color: grey;
}

button {
  border: 1px solid blue;
  background-color: blueviolet;
}
</style>
