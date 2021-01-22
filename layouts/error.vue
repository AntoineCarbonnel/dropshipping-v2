<template>
  <div id="error">
    <h1 class="content">ERROR {{ error.statusCode }}</h1>
    <div class="content">
      Oops,an error occurred! <br/>
      let us help you out
    </div>
    <div class="links">
      <NuxtLink to="./">Back</NuxtLink>
      <NuxtLink to="/">Home</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: "error",
  props: ['error'],
  layout: 'errorLayout'
}
</script>

<style scoped lang="scss">
div#error {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  > .content {
    margin: 0;
    font-size: 95px;
    text-align: center;
    font-weight: bold;
  }
  > .links {
    margin-top: 3vh;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 60%;

    > a {
      font-size: 24px;
      font-weight: bold;
      padding: 15px 50px;
      background-color: #FCEFEE;
    }
  }
}
</style>
