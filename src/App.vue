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
      <Services />
    </div>  

      <section id="footer">
        <Footer />
      </section>
      <router-view />
  </div>
</template>

<style>
  body{
    background-color: #0A1D3E;
    font-family: 'Montserrat', sans-serif;
  }
</style>

<script>

import Header from './components/header_exapmle.vue'
import Footer from './components/footer_example.vue'
import Company from './components/about_our_company.vue'
import Services from './components/services.vue'


export default{
  name: 'App',
  components: {
    Header,
    Company,
    Footer,
    Services,
  },
  methods: {
    scroll() {
      const element = document.getElementById('footer');
      element.scrollIntoView({ behavior: 'smooth' });
    }
  },

}

</script>
