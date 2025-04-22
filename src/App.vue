<script setup>
    import { ref } from "vue";

    const lancamentos1 = ref([
      {
        imagem: '../src/assets/books/cfi_vol2.png',
        titulo: 'Chsin of Iron: Volume 2',
        autor: 'Cassandra Clare',
        preco: 'R$23.24'

      },
      {
        imagem: '../src/assets/cft.png',
        titulo: 'Chain of Thorns',
        autor: 'Cassandra Clare',
        preco: 'R$23.24',

      },
      {
        imagem: '../src/assets/cofa.png',
        titulo: 'City of Fallen Angels',
        autor: 'Cassandra Clare',
        preco: 'R$13.94',
        coracao: '',

      },
      {
        imagem: '../src/assets/nonaTheNinth.png',
        titulo: 'Nona The Ninth',
        autor: 'Cassandra Clare',
        preco: 'R$16.84',
        coracao: '',
      }
     ])

    const lancamentos2 = ref([
      {
        imagem: '../src/assets/books/harlemS.png',
        titulo: 'Harlem Shuffle',
        autor: 'Colson Whitehead',
        preco: 'R$26.92',
        coracao: '',

      },
      {
        imagem: '../src/assets/two.png',
        titulo: 'Two Old Women',
        autor: 'Velma Wallis',
        preco: 'R$13.95',
        coracao: '',

      },
      {
        imagem: '../src/assets/carrie.png',
        titulo: 'Carrie Soto Is Back',
        autor: 'Taylor Jenkins Reid',
        preco: 'R$26.04',
        coracao: '',

      },
      {
        imagem: '../src/assets/bookLovers.png',
        titulo: 'Book Lovers',
        autor: 'Emily Henry',
        preco: 'R$15.81',
        coracao: '',
      }
     ])
</script>

<template>
  <header>
    <ul>
      <li>
        <h3>IFbooks</h3>
        <p><span>|</span></p>
        <p>Apreço a <br> leitura</p>
        <div>
          <input type="text" placeholder="Pesquisar">
          <img src="../src/assets/lupa.png" alt="">
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
          <span class="fa-solid fa-cart-shopping" style="color: #63E6BE;"></span>
          <span class="fa-solid fa-heart" style="color: #63E6BE;"></span>
          <span class="fa-solid fa-user" style="color: #63E6BE;"></span>
        </nav>
      </li>
    </ul>
  </header>

  <main>
    <section class="banner">
      <ul>
      <li>
        <button>Autor de Abril</button>
        <h1>Erick Manuel Scimitt</h1>
        <p>Eric-Emmanuel Schmitt has been awarded more than 20 literary prizes and distinctions, and in 2001 he received the title of Chevalier des Arts et des Lettres. His books have been translated into over 40 languages.</p>
        <button>Acessar Página do Livro</button>
      </li>
      <li>
        <img src="../src/assets/book.png" alt="">
        <p>*within the stock limit</p>
      </li>
    </ul>
    </section>

    <section class="holder">
      <img src="../src/assets/caminhão.png" alt=""> <p>|</p>
      <img src="../src/assets/estrela.png" alt=""> <p>|</p>
      <img src="../src/assets/livros.png" alt=""> <p>|</p>
    </section>

    <section>
      <h3>Lançamentos</h3>
      <div>
        <article v-for="lancamento in lancamentos1" :key="lancamento.id">
        <img :src="lancamento.imagem" alt="">
        <h2>{{ lancamento.titulo }}</h2>
        <p>{{ lancamento.autor }}</p>
      </article>
      </div>

      <div>

      </div>
    </section>

  </main>

  <footer>

  </footer>
</template>

<style scoped>

</style>
