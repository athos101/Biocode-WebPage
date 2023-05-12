<template>
<section class="container">
    <h1 class="title">Membros</h1>
    <div class="image-container">
      <img
        v-bind:src="images[currentImage]"
        class="{ 'animate__animated': shouldUpdateImage, 'animate__fadeOut': shouldUpdateImage }"
        @animationend="shouldUpdateImage = false"
        alt="imagemMembro"
        width="232"
        height="191"
        top="92"
        left="437"
      />
    </div>
    <div class="controls">
        <button @click="previousImage">
          <img src="../assets/arrow-left-solid.svg" alt="arrow-left" width="27" height="27">
          </button>
        <button @click="nextImage">
          <img src="../assets/arrow-right-solid.svg" alt="arrow-right" width="27" height="27">
        </button>
    </div>
</section>
    
</template>

<style scoped>

@import url("https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css");

.container{
   background-color: rgba(217, 217, 217, 0.1);;
    border-radius: 30px;
    height: 326px;
    width: 1072px;
    left: 184px;
    top: 1864px;

   
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.image-container {
   width: 232px; /* Largura desejada para a imagem */
  height: 191px; /* Altura desejada para a imagem */
  display: flex;
  align-items: center;
  justify-content: center;
  
  }


.title {
    color: #fff;
     position: relative;
     top: 0;
    margin-top: 0;
    font-size: 36px;
}

.controls{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 98%;
    position: relative;
}



button {
  background-color: transparent;
  border: none;
  outline: none;
  border-radius: 4px;
  padding: 8px 12px;
  cursor: pointer;

}

</style>


<script>
export default{
    name: 'Members',

data() {

    return{
    images: [
       require('../assets/perfil.png'),
        require('../assets/perfil.png'),
        require('../assets/perfil.png'),
    ],
    currentImage: 0,
    shouldUpdateImage: false
    };
},

methods: {
    previousImage() {
      this.currentImage = this.currentImage === 0 ? this.images.length - 1 : this.currentImage - 1;
      this.shouldUpdateImage = true;
    },
    nextImage() {
      this.currentImage = this.currentImage === this.images.length - 1 ? 0 : this.currentImage + 1;
      this.shouldUpdateImage = true;
    },
  },

}
</script>
