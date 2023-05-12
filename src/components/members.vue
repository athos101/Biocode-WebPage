<template>
  <h1 class="title">Membros</h1>
  <section class="container">
    <div class="content-wrapper">
      <div class="controls">
        <button @click="previousImage">
          <img src="../assets/arrow-left-solid.svg" alt="arrow-left" width="27" height="27">
        </button>
      </div>
      <div class="image-container">
        <transition name="fade" mode="out-in">
          <img
            :key="currentImage"
            v-bind:src="images[currentImage]"
            class="fade"
            alt="imagemMembro"
            style="height: 480px;"
            top="92"
            left="437"
          />
        </transition>
      </div>
      <div class="controls">
        <button @click="nextImage">
          <img src="../assets/arrow-right-solid.svg" alt="arrow-right" width="27" height="27">
        </button>
      </div>
    </div>
  </section>
</template>

<style scoped>

.container{
   background-color: rgba(217, 217, 217, 0.1);;
    border-radius: 30px;
    height: 600px;
    width: 1000px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin:auto;
    margin-bottom: 120px;
}

.content-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

.image-container {
   margin-right: 0 20px;
   flex-flow: 1;
  }

  #images {
    opacity: 1;
  }
  
  .fade-enter-active,
.fade-leave-active {
  transition: opacity 0.2s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}



.title {
    color: #fff;
     position: relative;
     top: 0;
    margin-bottom: 80px;
    font-size: 36px;
    margin-left: 5%;
}

.controls{
    display: flex;
    filter: invert(100%);
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
export default {
  name: 'Members',
  data() {
    return {
      images: [
        require('../assets/mimikyu.png'),
        require('../assets/mimikyu.png'),
        require('../assets/mimikyu.png'),
      ],
      currentImage: 0,
    };
  },
  methods: {
    previousImage() {
      this.currentImage = this.currentImage === 0 ? this.images.length - 1 : this.currentImage - 1;
    },
    nextImage() {
      this.currentImage = this.currentImage === this.images.length - 1 ? 0 : this.currentImage + 1;
    },
  },
};

</script>
