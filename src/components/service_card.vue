<template>
    <div class="card">
      <div class="card-content">
        <!-- Your card content here -->
        <slot>{{ textoDevMobile }}</slot>
      </div>
    </div>
  </template>
  
  <style>
  .card {
    margin: 20px;
    background-color: rgba(255, 255, 255, 0);
    border: 1px solid #FFFFFF;
    height: 250px;
  }
  
  .card-content {
    padding: 10px;
  }
  </style>

<script>
  export default{
    data(){
      return{
        textoDevMobile: 'A praticidade dos dispositivos móveis e a internet diminuem a distância entre pessoas e serviços. Por isso, desenvolvemos aplicativos que sirvam de ferramenta para o trabalho em saúde, comunicação, automatização de processos, registro e muito mais.',
      }
    }
  }
</script>