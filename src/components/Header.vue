<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: "header",
  data() {
    return {
      title: "Vue.js Demo"
    };
  }
};
</script>

<style scoped>
header {
  width: 100%;
  background: #333;
  padding: 6px;
}

h1 {
  color: lightgreen;
  text-align: center;
 
}
</style>