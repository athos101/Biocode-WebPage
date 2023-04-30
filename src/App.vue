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
  }
</style>

<script>

import Header from './components/header_exapmle.vue'
import Footer from './components/footer_example.vue'
import Company from './components/about_our_company.vue'
import {createWebHistory, createRouter} from "vue-router"


export default{
  name: 'App',
  components: {
    Header,
    Company,
    Footer,
  },
  methods: {
    scroll() {
      const element = document.getElementById('footer');
      element.scrollIntoView({ behavior: 'smooth' });
    }
  },

}

</script>
