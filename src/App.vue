<script setup>
import { ref } from "vue";

const content = ref({
  header: "Header content here.",
  main: "Main content here.",
  footer: "Footer content here.",
});
</script>

<template>
  <div>
    <header class="header">{{ content.header }}</header>

    <main class="main">
      <div>{{ content.main }}</div>
    </main>

    <footer class="footer">{{ content.footer }}</footer>
  </div>
</template>

<style scoped>
.header,
.footer {
  display: block;
  text-align: center;
  padding: 24px;
  font-size: 24px;
  color: darkgreen;
  background-color: aquamarine;
}
.main {
  display: block;
  justify-items: center;
  align-content: center;
  margin: 36px;
  height: 50vh;
  padding: 24px;
  background-color: skyblue;
  color: blue;
}
</style>
