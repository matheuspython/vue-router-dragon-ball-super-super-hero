<template>
  <TheHeader />
  <router-view />
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
export default {
  components: { TheHeader },
};
</script>

<style>
:root {
  --backgrond: #000;
  --text-color: #fff;
  --button: #8257e5;
  --border: #29292e;
  --border-menu-mobile: #a8a8b3;
  --text-color-menu-mobile: #e1e1e6;
  --secondary: #2f3136;
  --tertiary: rgb(32, 34, 37);
}
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html,
body {
  height: 100%;
}
body {
  background: var(--backgrond);
  color: var(--text-color);
}
a {
  color: var(--text-color);
  text-decoration: none;
}
#app {
  font-family: "Roboto", sans-serif, Avenir, Helvetica, Arial;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
ul {
  list-style-type: none;
}
.container{
  width: 100%;
  max-width: 1280px;
  margin: 0 auto;
}
</style>
