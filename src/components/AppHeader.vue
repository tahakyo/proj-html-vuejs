<template>
  <div class="container">
    <div class="nav">
      <div class="nav__logo">
        <img src="../assets/img/logo-2.png" alt="header-logo">
      </div>
      <ul class="nav__menu">
          <li><a href="">menu#</a></li>
          <li><a href="">menu#</a></li>
          <li><a href="">menu#</a></li>
          <li><a href="">menu#</a></li>
          <li><a href="">menu#</a></li>
      </ul>
      <div class="nav__actions">
        <i class="fas fa-search"></i>
        <i class="fas fa-shopping-cart"></i>
      </div>
      <div class="nav__button">
        <a class="myButton" href="#">Get Started</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader"
}
</script>

<style lang="scss" scoped>
.nav {
  display: flex;
  width: 100%;
  &__logo {
    width: 20%;
    display: flex;
    align-items: center;
    img {
      width: 2rem;
    }
  }
  &__menu {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 50%;
  }
  &__actions {
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 10%;
  }
  &__button {
    margin-left: auto;
    a {
      color: white;
    }
    
  }
}
</style>