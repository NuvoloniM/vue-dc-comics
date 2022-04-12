<template>
  <div id="app">
    <header>
      <NavComp/>
    </header>
    <main>
      <ContentComp/>
      <HeroNavComp/>
    </main>
    <footer>
      <div></div>
      <div></div>
      <div></div>
    </footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import NavComp from './components/NavComp.vue';
import ContentComp from './components/ContentComp.vue';
import HeroNavComp from './components/HeroNavComp.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld
    NavComp,
    ContentComp,
    HeroNavComp,
  }
}
</script>

<style lang="scss">

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
