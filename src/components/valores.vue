<template>
  <h1 class="title">Valores</h1>
  <section class="container">
    <div class="icon-container">
      <img src="..\assets\scale-balanced-solid.svg" alt="">
      <p>Ética</p>
    </div>
    <div class="icon-container">
      <img src="..\assets\award-solid.svg" alt="">
      <p>Qualidade</p>
    </div>
    <div class="icon-container">
      <img src="..\assets\lightbulb-regular.svg" alt="">
      <p>Inovação</p>
    </div>
    <div class="icon-container">
      <img src="..\assets\handshake-angle-solid.svg" alt="">
      <p>Colaboração</p>
    </div>
    <div class="icon-container">
      <img src="..\assets\magnifying-glass-solid.svg" alt="">
      <p>Transparência</p>
    </div>
  </section>
</template>

<style scoped>
.title {
  color: #fff;
  position: relative;
  top: 0;
  margin-bottom: 80px;
  font-size: 36px;
  margin-left: 5%;
}

.container {
  padding: 30px;
  margin: 120px;
  background: rgba(217, 217, 217, 0.1);
  border-radius: 30px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.icon-container {
  flex-basis: 20%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #fff;
}

.icon-container img {
  width: 50px;
  height: 50px;
  filter: invert(100%);
}

.icon-container p {
  font-size: 20px;
  margin-top:  50px;
}
</style>

<script>
export default {
  name: 'Valores',
}
</script>
