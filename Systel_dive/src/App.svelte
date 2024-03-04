<!-- App.svelte -->
<script>
  import Navbar from './components/Navbar.svelte';

  let fondodepantalla = 'fondo';
  let src = '/img/fondoDePantalla.jpg'
</script>

<main>
  <img {src} alt="{fondodepantalla} fondo" />
  <Navbar/>
  
  <!-- Aquí colocarías el resto de tu aplicación -->
</main>

<style>
  /* Estilos globales de tu aplicación */
  main {
    padding: 20px;
    background-image: url(fondoDePantalla.jpg);
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
  }
</style>

