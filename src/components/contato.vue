<template>

<div class="container">
    <div class="column">
        <p class="title">ENTRE EM CONTATO</p>
        <p class="contato">biocodejr@ufcspa.edu.br</p>
        <p class="contato">@biocodejr</p>

    </div>

    <div class="column">

          <form>
            <div class="form-group">
            <input type="text" class="form-control custom-font" style="margin-top: 80px;" id="nome" placeholder="Digite seu nome" name="nome" required>
            </div>
            
            <div class="form-group">
            <input type="email" class="form-control custom-font" id="email" placeholder="Digite seu email" name="email" required>
            </div>
            
            <div class="form-group">
            <input type="text" class="form-control custom-font" id="assunto" placeholder="Digite o assunto" name="assunto" required>
            </div>

            <div class="form-group">
            <textarea id="mensagem" class="form-control custom-font" placeholder="Digite a mensagem" name="mensagem" rows="15" required></textarea>
            </div>

            <div class="form-group">
            <button type="submit" class="botao">Enviar</button>
            </div>
          </form>
      
    </div>
  </div>



  </template>

<style scoped>

.container {
  display: flex;
  flex-direction: row;
  margin: 120px;
}

.column {
  color: #ffffff;
  flex: 1;
  margin: 20px;
  display: flex;
  flex-direction: column;
}

.title{
    font-size: 70px;
    margin-bottom: 80px;
}

.contato{
    font-size: 15px;
    margin-bottom: 0px;
}

.custom-font {
  font-size: 15px;
  font-style: Arial;
  margin-bottom: 10px;
  width: 100%;
  padding: 5px;
}

.botao {
  background-color: #8F0C3C;
  color: #ffffff;
  border: none;
  width: 100px;
  padding: 15px;
  border-radius: 10px;
  font-size: 20px;
}

.botao:hover{
  background-color: #F84D80;
  /* color: #ffffff; */
  transition: 0.5s;
}

</style>
  