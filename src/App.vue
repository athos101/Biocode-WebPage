<template>
  <div id="app">
    <!-- <Header /> -->
    <header>
      <div class="logo-container">
    <img src="./assets/blogo.png" alt="Logo" height="60" width="60">
    <h1 class="title">BIOCODE JR</h1>
  </div>
      <nav class="header_nav">
        <ul>
          <li><a @click="scrollToSection('company-section')" style="cursor: pointer;">Quem somos</a></li>
          <li><a @click="scrollToSection('services-section')" style="cursor: pointer;">Serviços</a></li>
          <li><a @click="scrollToSection('contato-section')" style="cursor: pointer;">Contato</a></li>
        </ul>
        
      </nav>
     
    </header>
    
        
       
    <div id="body">
<<<<<<< HEAD
=======
     <Company id="company-section" />
     <Historia id="historia-section" />
      <Services id="services-section" />
     <Contato id="contato-section" />
>>>>>>> 3005b1d3a5940bdeb763a8d82fa3195cc5bacb22
    </div>  

      <section id="footer">
        <Footer />
      </section>
      <router-view />
  </div>
</template>

<style>

body{
        padding: 0;
        margin: 0;

      }
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
    
    scrollToSection(sectionId) {
      const element = document.getElementById(sectionId);
      element.scrollIntoView({ behavior: 'smooth' });
    }
    
  },
 
  

}

</script>
