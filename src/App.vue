<script setup></script>

<template>
  <header>
    <ul>
      <li>
        <h3>IFbooks</h3>
        <p><span>|</span></p>
        <p>
          Apreço a <br />
          leitura
        </p>
        <div>
          <input type="text" placeholder="Pesquisar" />
          <img src="../src/assets/lupa.png" alt="" />
        </div>
      </li>
      <li>
        <nav>
          <a href="">Termos</a>
          <a href="">Equipe</a>
          <a href="">Envio</a>
          <a href="">Devoluções</a>
        </nav>
        <nav>
          <RouterLink to="/carrinho">
            <span class="fa-solid fa-cart-shopping" style="color: #63e6be"></span> carrinho
          </RouterLink>
          <span class="fa-solid fa-heart" style="color: #63e6be"></span>
          <span class="fa-solid fa-user" style="color: #63e6be"></span>
        </nav>
      </li>
    </ul>
  </header>

  <router-view></router-view>

  <footer>
    <div class="footer">
      <div>
        <ul>
          <p>IFbooks</p>
          <li>
            <span class="fa-brands fa-square-facebook"></span>
            <span class="fa-brands fa-square-instagram"></span>
            <span class="fa-brands fa-square-x-twitter"></span>
          </li>
        </ul>
      </div>
      <div>
        <h3>Contatos</h3>
        <ul>
          <li>
            <span class="fa-solid fa-phone"></span>
            <p>+55 47 40045263</p>
          </li>
          <li>
            <span class="fa-solid fa-clock"></span>
            <p>8h às 23h - Seg a Sex</p>
          </li>
          <li>
            <span class="fa-solid fa-envelope"></span>
            <p>contato@ifbooks.com</p>
          </li>
        </ul>
        <img src="../src/assets/ways to pay.png" alt="" />
      </div>
    </div>
    <p>© Alguns direitos reservados. IFbooks 2025.</p>
  </footer>
</template>

<style scoped></style>
