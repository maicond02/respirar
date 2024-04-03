<template>
  <footer>
    <div class="footer-container">
      <div class="footer-column">
        <h3>Sobre Nós</h3>
        <p>Somos uma empresa dedicada a fornecer soluções digitais inovadoras.</p>
      </div>
      <div class="footer-column">
        <h3>Links Rápidos</h3>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Sobre</a></li>
          <li><a href="#">Serviços</a></li>
          <li><a href="#">Contato</a></li>
        </ul>
      </div>
      <div class="footer-column">
        <h3>Contato</h3>
        <p>Endereço: Rua Exemplo, 123<br>
           Cidade Exemplo<br>
           Telefone: (00) 1234-5678<br>
           Email: exemplo@email.com</p>
      </div>
      <div class="footer-column">
        <h3>Redes Sociais</h3>
        <div class="social-media-icons">
          <a href="#"><i class="fab fa-facebook-f"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
          <a href="#"><i class="fab fa-linkedin-in"></i></a>
        </div>
      </div>
    </div>
    <p>&copy; 2024 Exemplo de Footer. Todos os direitos reservados.</p>
  </footer>
</template>

<style scoped>
    footer {
    background-color: #18181b;
    color: #fff;
    padding: 40px 20px;
    text-align: center;
    bottom: 0;
    width: 100%;
  }
  
  .footer-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  
  .footer-column {
    flex: 1;
    padding: 0 20px;
  }
  
  .footer-column h3 {
    font-size: 20px;
    margin-bottom: 20px;
    color: #fff;
  }
  
  .footer-column ul {
    list-style: none;
    padding: 0;
  }
  
  .footer-column ul li {
    margin-bottom: 10px;
  }
  
  .footer-column ul li a {
    color: #fff;
    text-decoration: none;
  }
  
  .social-media-icons {
    margin-top: 20px;
  }
  
  .social-media-icons a {
    color: #fff;
    margin-right: 10px;
    font-size: 20px;
  }
</style>