<template>
    <section class="about">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <h2>About Our Company</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor velit quis tortor molestie, sed blandit quam efficitur. Donec quis bibendum nisi. Praesent tincidunt lorem id arcu pellentesque, non euismod nulla imperdiet. Duis sed mollis quam. Mauris interdum eros sed nisi iaculis, vel faucibus enim tincidunt. Integer vel nunc et sapien faucibus mollis a in mi.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor velit quis tortor molestie, sed blandit quam efficitur. Donec quis bibendum nisi. Praesent tincidunt lorem id arcu pellentesque, non euismod nulla imperdiet.</p>
            <a href="#" class="btn btn-primary">Learn More</a>
          </div>
          <div class="col-md-6">
            <img src="/path/to/image.jpg" alt="Company Image">
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <style>
  .about {
    /* background-color: #f9f9f9; */
    padding: 3rem 0;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }
  
  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
  
  .col-md-6 {
    width: 50%;
    padding: 1rem;
    box-sizing: border-box;
  }
  
  h2 {
    color: #ffffff;
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
  }
  
  p {
    color: #ffffff;
    font-size: 1.2rem;
    line-height: 1.5;
    margin-bottom: 1.5rem;
  }
  
  .btn {
    display: inline-block;
    padding: 1rem 2rem;
    background-color: #333333;
    color: #ffffff;
    border: none;
    border-radius: 4px;
    font-size: 1.2rem;
    text-decoration: none;
    transition: background-color 0.3s ease;
  }
  
  .btn:hover {
    background-color: #222222;
  }
  </style>
  