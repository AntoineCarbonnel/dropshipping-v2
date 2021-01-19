<template>
  <div>
    <header>
      <div class="equalizer"></div>
      <h1>{{ title }}</h1>
      <nav>
        <div>
          <img src="~/assets/img/basket.png" alt="Basket logo">
        </div>
        <div>
          <img src="~/assets/img/wish.png" alt="Wishlist logo">
        </div>
        <div>
          <img src="~/assets/img/account.png" alt="Account logo">
        </div>
      </nav>
    </header>
    <Nuxt/>
  </div>
</template>
<script>
export default {
  name: 'Header',
  data() {
    return {
      title: 'QueensNeverGetCold'
    }
  }
}

</script>
<style lang="scss">
body{
  font-family: 'Montserrat', sans-serif;
  margin: 0;
}
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;

  .equalizer {
    width: 10vw;
  }

  h1 {
    font-size: 40px;
    font-weight: 600;
  }

  nav {
    display: flex;
    width: 10vw;
  }
}

</style>
