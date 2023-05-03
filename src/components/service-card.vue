<template>
    <div class="card">
      <img :src="require('@/assets/' + item)" :alt="item">
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
    height: 300px;
    border-radius: 20px;

    display: flex;
    flex: 1;
    flex-direction: row;
    text-align: center;
  }

  .card img{
    align-self: center;
    padding-left: 15px;
    padding-right: 15px;
    width: 200px;
    height: 200px;
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

  }
</script>