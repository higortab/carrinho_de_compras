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
        imagem: '../src/assets/books/cft.png',
        titulo: 'Chain of Thorns',
        autor: 'Cassandra Clare',
        preco: 'R$23.24'

      },
      {
        imagem: '../src/assets/books/cofa.png',
        titulo: 'City of Fallen Angels',
        autor: 'Cassandra Clare',
        preco: 'R$13.94',
        coracao: '',

      },
      {
        imagem: '../src/assets/books/nonaTheNinth.png',
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
        imagem: '../src/assets/books/two.png',
        titulo: 'Two Old Women',
        autor: 'Velma Wallis',
        preco: 'R$13.95',
        coracao: '',

      },
      {
        imagem: '../src/assets/books/carrie.png',
        titulo: 'Carrie Soto Is Back',
        autor: 'Taylor Jenkins Reid',
        preco: 'R$26.04',
        coracao: '',

      },
      {
        imagem: '../src/assets/books/bookLovers.png',
        titulo: 'Book Lovers',
        autor: 'Emily Henry',
        preco: 'R$15.81',
        coracao: '',
      }
     ])
</script>

<template>

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
        <p>{{ lancamento.preco }}</p>
        <button>Comprar</button>
      </article>
      </div>

      <div>
        <article v-for="lancamento in lancamentos2" :key="lancamento.id">
        <img :src="lancamento.imagem" alt="">
        <h2>{{ lancamento.titulo }}</h2>
        <p>{{ lancamento.autor }}</p>
        <p>{{ lancamento.preco }}</p>
        <button>Comprar</button>
      </article>
      </div>
    </section>

  </main>

 
</template>

<style scoped>

</style>
