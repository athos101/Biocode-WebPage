<template>
    <section class="about">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
           <!-- <h2>Seção Inicial</h2> -->
            <p class="nameBioCode">BIOCODE JR</p>
            <p class="content"> Inovação e tecnologia nas áreas de Informática em Saúde e Bioinformática.</p>
            <!--<a href="#" class="btn btn-primary">Learn More</a>-->
          </div>
            <!--<img src="/path/to/image.jpg" alt="Company Image">-->
            <!--<img src="../assets/BioCode.png" alt="Imagem teste" height="100" width="100">-->
            <!--<img src="../assets/biocodejr-hero1.png" alt="Imagem teste" height="300" width="400">-->
            <div class="imgs">
              <img class="tech" src="../assets/tecnologia.png" alt="Imagem teste" width="60%">
              <img class="health" src="../assets/healthy.png" alt="Imagem teste" width="60%">
            </div>
        </div>
      </div>
    </section>
  </template>

  <style>
  .nameBioCode {
    color: #ffffff;
    font-size: 70px;
    margin-bottom: 80px;
    /* font-family: fantasy; */

  }

  .container {
    max-width: 95%;
  }
  
  .row {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
  
  .col-md-6 {
    /* width: 20%; */
    padding: 1rem;
    margin-top: 200px;
    margin-left: 8%;
    box-sizing: border-box;
    display: flex;
    flex: 1;
    flex-direction: column;
  }
  
  h2 {
    color: #ffffff;
    font-size: 2.8rem;
    margin-bottom: 1.5rem;
    display: flex;
  }

  .content {
    color: #ffffff;
    font-size: 1.6rem;
    line-height: 1.5;
    margin-bottom: 1.5rem;
    display: flex;
  }
  
  .imgs{
    width: 40%;
    align-content: end;
    margin-top: 200px;
    margin-left: 5%;
    margin-right: 10%;
    display: flex;
    flex: 1;
  }

  .health{
    margin-left: 10%;
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
  