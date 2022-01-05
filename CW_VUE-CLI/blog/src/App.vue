<template>
  <nav class="nav">
    <router-link class="link nav__link" to="/catalog">Товары</router-link>
    <router-link class="link nav__link" to="/cart">Корзина: {{ this.$store.getters.cartCount }}
    </router-link>
  </nav>
  <router-view/>
</template>
<style>
.nav {
  text-align: center;
  margin-bottom: 18px;
}
.link {
  text-decoration: none;
  color: #864b4b;
}
.link:hover {
  color: #554f4f;
}
.nav__link {
  font-size: 1.5rem;
  padding: 0 10px;
}
</style>