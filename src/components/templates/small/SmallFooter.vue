<script setup></script>
<template>
  <div id="footerMenu" :style="{ display: showMenu ? 'block' : 'none' }">
    <RouterLink to="/">
      <i class="mdi mdi-home-outline" size="25" fillColor="#282828" /> Home
    </RouterLink>
    <RouterLink to="/login">
      <i class="mdi mdi-account" /> Login
    </RouterLink>
  </div>
  <div class="icons">
    <RouterLink to="/">
      <i class="mdi mdi-home-outline" />Home
    </RouterLink>
    <RouterLink to="/">
      <i class="mdi mdi-account-circle-outline" />Perfil
    </RouterLink>
    <RouterLink to="/">
      <i class="mdi mdi-cart-outline" />Carrinho
    </RouterLink>
    <div class="hamburger" @click="showMenu = !showMenu">
      <Menu size="25" fillColor="#282828" />Menu
    </div>
  </div>
</template>
<style scoped>
#footerMenu {
  position: fixed;
  bottom: 15%;
  right: 0;

  width: 20%;
  border-top: #eeeeee 1px solid;
  background-color: white;

  display: block;
  padding: 1rem;
}

#footerMenu a {
  display: flex;
  width: 100%;
  justify-content: space-between;
  text-decoration: none;
  color: #282828;
  font-size: 1rem;
  transition: color 0.3s;
}

.icons {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: space-between;
  font-size: 1.7rem;
}

.icons a {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-decoration: none;
  color: #282828;
  font-size: 1rem;
  transition: color 0.3s;
}
</style>