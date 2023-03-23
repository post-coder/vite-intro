<script>
export default {
  data() {
    return {
      links: ["link 1", "link 2", "link 3"],
    };
  },
};
</script>

<template>
  <nav>
    <ul>
      <li v-for="link in links">{{ link }}</li>
    </ul>
  </nav>
</template>

<style>
nav {
  /* color: green; */
  border-bottom: 1px white solid;
}

ul {
  display: flex;
  flex-flow: row;
  gap: 10px;
  list-style-type: none;
}
</style>
