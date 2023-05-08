<template>
    <footer class="footer">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <p>&copy; 2023 My Company</p>
          </div>
          <div class="col-md-6">
            <nav>
              <ul>
                <li><a href="#">Terms of Service</a></li>
                <li><a href="#">Privacy Policy</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
export default {
  name: "Footer",
};
</script>

  <style>
  footer {
    background-color: #333;
    color: #fff;
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
  
  nav ul {
    list-style: none;
    display: flex;
    justify-content: flex-end;
    margin: 0;
    padding: 0;
  }
  
  nav li {
    margin-left: 2rem;
  }
  
  nav a {
    color: #fff;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.3s ease;
  }
  
  nav a:hover {
    color: #b34040;
  }
  </style>
  