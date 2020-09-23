<template>
  <div id="app">
    <Header/>
    <nav>
      <router-link class="menu" to="/">Início</router-link>
      <router-link class="menu" to="/sobre">Sobre</router-link>
    </nav>

    <main>
      <transition name="scale" mode="out-in">
        <router-view/>
      </transition>
    </main>

    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="scss">
@import "./assets/css/estilo.scss";
</style>
