<template>
<header>
  <div class="logo">Logo Here</div>
  <nav class="header_nav">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
  <div class="cta">
    <button>Sign Up</button>
  </div>
</header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: #ffffff;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}

.logo {
  font-size: 2rem;
  font-weight: bold;
}

.header_nav ul {
  display: flex;
  list-style: none;
  margin: 0;
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

.cta button {
  padding: 1rem 2rem;
  border-radius: 4px;
  background-color: #333333;
  color: #ffffff;
  font-size: 1.2rem;
  border: none;
  cursor: pointer;
}

.cta button:hover {
  background-color: #222222;
}
</style>