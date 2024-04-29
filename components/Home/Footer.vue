<template>
  <footer>
    <div class="footer-container">
      <div class="footer-column">
        <h3>Sobre Nós</h3>
        <p>O <strong>RespirAr</strong> é o mais novo sistema de monitoramento da qualidade do ar, projetado para fornecer dados precisos e em tempo real sobre a qualidade do ar em sua comunidade.</p>
      </div>
      <div class="footer-column">
        <h3>Links Rápidos</h3>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">Sobre</a></li>
          <li><a href="/buy">Serviços</a></li>
          <li><a href="/contact">Contato</a></li>
        </ul>
      </div>
      <div class="footer-column">
        <h3>Contato</h3>
        <p>Endereço: Rua Exemplo, 123<br>
           Americana - SP<br>
           Telefone: (00) 1234-5678<br>
           Email: respirar@email.com</p>
      </div>
      <div class="footer-column">
        <h3>Redes Sociais</h3>
        <div class="social-media-icons">
          <a href="#"><i class="pi pi-whatsapp"></i></a>
          <a href="#"><i class="pi pi-facebook"></i></a>
          <a href="#"><i class="pi pi-instagram"></i></a>
          <a href="#"><i class="pi pi-twitter"></i></a>
        </div>
      </div>
    </div>
    <p>&copy; 2024 Respirar. Todos os direitos reservados.</p>
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