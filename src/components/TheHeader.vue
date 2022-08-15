<template>
  <header>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
    header {
        width: 100%;
        height: 50px;
        margin-top: 30px;
    }
    header nav{
        width: 100%;
        margin: 0 auto;
        max-width: 1280px;
        padding: 0 2%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 15px;
    }
</style>
