<template>
  <div id="app">
    <headbar></headbar>
    <div class="body">
      <carousal></carousal>
      <highlights></highlights>
    </div>
  </div>
</template>

<script>
import hello from "./components/HelloWorld.vue";
import carousal from "./components/carousal.vue";
import headbar from "./components/headbar.vue";
import highlights from "./components/highlights.vue"

export default {
  name: "app",
  components: {
    hello,
    headbar,
    carousal,
    highlights
  }
};
</script>

<style>

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
*{
  box-sizing: border-box;
}

.body {
  /* background-color: blue; */
  margin-top: 2ch;
  /* display: flex;
  flex-direction: column; */
}

</style>
