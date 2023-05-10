<template>
<header>
  <div class="logo-container">
    <img src="../assets/blogo.png" alt="Logo" height="60" width="60">
    <h1 class="title">BIOCODE JR</h1>
  </div>
  <nav class="header_nav">
    <ul>
      <li><a href="#">Quem somos</a></li>
      <li><a href="#">Serviços</a></li>
      <li><a href="#">Contato</a></li> 
       
    </ul>
  </nav>
 
</header>
</template>

<script>
export default {
  name: "Header",
 
};
</script>

<style>
header {
  position: fixed;
  width: 100%;
  height: 65px;
  top: 10;
  z-index: 999;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: #E11955;
  
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}

.logo-container {
  margin-left: 200px;
  display: flex;
  align-items: center;
}

.logo {
  margin-top: 0.2%;
  margin-left: 10%;
  font-size: 2rem;
  font-weight: bold;
}

.title {
  margin-left: 100px;
  color: white;
  font-size: 30px;
  margin: 0;
  
}

.header_nav ul {

  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-right: 120px;
  padding: 0;
}

.header_nav li {
  margin-right: 1rem;
}

nav li:last-child {
  margin-right: 0;
}

.header_nav a {
  color: #333333;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.2rem;
}

.header_nav a:hover{
    color: rgb(42, 131, 131)
}



</style>