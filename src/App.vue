<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from "./pages/Home";

export default {
  name: "App",
  components: {
    Home
  }
};
</script>

<style>
html {
  height: 100%;
  width: 100%;
}
body {
  height: 100%;
  width: 100%;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100%;
}
</style>
