<script setup lang="ts">
import localStorageContent from "../pages/cart.vue";
</script>

<template>
  <header class="headerPage"><!--header -->

    <div class="homeButton">
      <a>
        <h2>
          <router-link to="/">Vuecommerce</router-link>
        </h2>
      </a>
    </div>
    <nav class="navbar"><!--navbar-->
      <ul class="headerList">

        <li>
          <router-link to="/cart">Carrinho</router-link>
        </li>

        <li>
          <router-link to="/about">About</router-link>
        </li>

      </ul>
    </nav><!--navbar final-->
  </header><!--header final-->
</template>

<style>
.headerPage {
    background-image: linear-gradient(rgb(255, 28, 28), rgb(219, 89, 89));
    width: 100%;
    display: flex;
    justify-content: space-between;
  }

  .homeButton {
    color: white;
  }

  .navbar {
    width: 40%;
  }

  .headerList {
    align-items: right;
    display: flex;
  }

  .headerList li {
    list-style: none;
    padding: 1rem 5rem;
    font-size: 16px;
    color: white;
  }

  .headerList li:hover {
    background: rgb(255, 47, 47);
    cursor: pointer;
    transition: all 0.5s;
  }
</style>