<template>
    <section class="about">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
           <!-- <h2>Seção Inicial</h2> -->
            <p class="nameBioCode">BIOCODE JR</p>
            <p> Atuamos nas áreas de Informática em Saúde e Bioinformática.</p>
            <!--<a href="#" class="btn btn-primary">Learn More</a>-->
          </div>
          <div class="col-md-6">
            <!--<img src="/path/to/image.jpg" alt="Company Image">-->
            <!--<img src="../assets/BioCode.png" alt="Imagem teste" height="100" width="100">-->
            <!--<img src="../assets/biocodejr-hero1.png" alt="Imagem teste" height="300" width="400">-->
            <img src="../assets/tecnologia.png" alt="Imagem teste" height="300" width="300">
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

  .nameBioCode {
    font-size: 70px;
    margin-bottom: 80px;
    font-family: fantasy;

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
  