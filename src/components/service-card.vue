<template>
    <div class="card">
      <img :src="require('@/assets/' + item)" :alt="item" :style="filter=imageFilter" @mouseover="imageFilter = '#F84D80'" @mouseout="imageFilter = 'none'">
      <div class="card-content">
        <!-- Your card content here -->
        <h1>{{ title }}</h1>
        <slot>{{ text }}</slot>
      </div>
    </div>
  </template>
  
  <style scoped>
    .card {
      margin: 20px;
      padding: 10px;

      background-color: rgba(255, 255, 255, 0);
      border: 2px solid #FFFFFF;
      border-radius: 20px;
      display: flex;
      text-align: center;
    }

    .card img{
      align-self: center;
      padding-left: 15px;
      padding-right: 15px;
      width: 170px;
      height: 180px;
      transition: 0.5s;
    }

    .card img:hover{
      filter: invert(60%) sepia(20%) saturate(3207%) hue-rotate(300deg) brightness(95%) contrast(100%);
      transition: 0.5s;
    }
    
    .card-content {
      display: flex;
      flex-direction: column;
      
      padding: 10px;
      font-size: 16px;
      color: #FFFFFF;
    }
    
    .card-content h1{
      font-size: 28px;
    }
  </style>

<script>
  export default{
    name: 'ServiceCard',
    props: {
      title: String,
      text: String,
      item: String,
    },
    data() {
      return {
        imageFilter:'none'
      }
    },

  }
</script>