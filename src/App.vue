<template>
  <div id="app">
    <!-- <Header /> -->
    <header>
      <div class="logo">Logo Here</div>
      <nav class="header_nav">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a @click="scroll" style="cursor: pointer;">Footer</a></li>
        </ul>
      </nav>
      <div class="cta">
        <button>Sign Up</button>
      </div>
    </header>
    <div id="body">
      <Company />
      <Company />
      <Historia />
      <Services />
      <Contato />
    </div>  

      <section id="footer">
        <Footer />
      </section>
      <router-view />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

import Header from './components/header_exapmle.vue'
import Footer from './components/footer_example.vue'
import Company from './components/about_our_company.vue'
import Services from './components/services.vue'
import Contato from './components/contato.vue'
import Historia from './components/historia.vue'

export default{
  name: 'App',
  components: {
    Header,
    Company,
    Footer,
    Services,
    Contato,
    Historia,
  },
  methods: {
    scroll() {
      const element = document.getElementById('footer');
      element.scrollIntoView({ behavior: 'smooth' });
    }
  },

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
