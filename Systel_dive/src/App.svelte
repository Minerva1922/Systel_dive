<script>
  let isOpen = false;

  function toggleNavbar() {
    isOpen = !isOpen;
  }
</script>

<nav class:open={isOpen} class="navbar">
  <button on:click={toggleNavbar} class="toggle-btn">
    ☰
  </button>
  <ul>
    <li><a href="/quienes-somos">Quienes somos</a></li>
    <li><a href="/que-hacemos">Que hacemos</a></li>
    <li><a href="/camaras">Cámaras</a></li>
    <li><a href="/contacto">Contacto</a></li>
  </ul>
</nav>

<style>
  .navbar {
    width: 200px;
    height: 100%;
    background-color: #333;
    position: fixed;
    top: 0;
    left: -200px;
    transition: left 0.3s ease;
  }

  .open {
    left: 0;
  }

  .toggle-btn {
    background: none;
    border: none;
    color: rgb(3, 3, 3);
    font-size: 1.5rem;
    cursor: pointer;
  }

  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  li {
    padding: 10px;
  }

  a {
    color: rgb(7, 7, 7);
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }
</style>

