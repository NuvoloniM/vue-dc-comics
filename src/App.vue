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
      <div class="footer-menu">
        <FooterComp/>
      </div>
      <div class="footer-social">
        <FooterMediaComp/>
      </div>
    </footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import NavComp from './components/NavComp.vue';
import ContentComp from './components/ContentComp.vue';
import HeroNavComp from './components/HeroNavComp.vue';
import FooterComp from './components/FooterComp.vue';
import FooterMediaComp from './components/FooterMediaComp.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld
    NavComp,
    ContentComp,
    HeroNavComp,
    FooterComp,
    FooterMediaComp
  }
}
</script>

<style lang="scss">

@import './assets/style/variables.scss';

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.footer-menu {
  background-image: url(./assets/img/footer-bg.jpg);
}

.footer-social {
  background: #373939;
  padding: 10px 0;
}
</style>
