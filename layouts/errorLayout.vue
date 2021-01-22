<template>
  <section>
    <Nuxt/>
  </section>
</template>

<script>
export default {
  name: "errorLayout"
}
</script>

<style scoped>
section {
  background-image: url("~assets/img/bg-errorpage.png");
  background-position: center top;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
