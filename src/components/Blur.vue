<template>
  <div class="blur"></div>
</template>

<script>
export default {
    name: 'BlurVue'
}
</script>

<style scoped>
.blur {
  overflow: hidden;
  position: absolute;
  background: #996dff;
  filter: blur(250px);
  width: 321px;
  height: 321px;
  border-radius: 50%;
}
</style>
Footer