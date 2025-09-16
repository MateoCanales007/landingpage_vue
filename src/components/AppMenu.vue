<template>
  <nav class="navbar">
    <div class="logo-container">
      <img src="@/assets/logo.png" alt="Logo" class="logo-img" />
      <span class="logo-text"> Landing Page</span>
    </div>
    <ul class="nav-links">
      <li><a href="https://vuejs.org/guide/introduction.html" target="_blank">Introduccion</a></li>
      <li><a href="https://router.vuejs.org/" target="_blank">Libreria</a></li>
      <li><a href="https://vuejs.org/guide/quick-start.html" target="_blank">Inicio Rapido</a></li>
      <li><a href="https://github.com/vuejs/" target="_blank">Github</a></li>
    </ul>
  </nav>
</template>

<style scoped>
/* Barra de navegación */
.navbar {
  background: #ffffff; /* azul */
  color: rgb(0, 0, 0);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 40px;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
}

/* Logo */
.logo-container {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo-img {
  height: 35px; /* tamaño del logo */
  width: 35px;
  object-fit: contain;
}

.logo-text {
  font-size: 1.3rem;
  font-weight: bold;
}

/* Links */
.nav-links {
  list-style: none;
  display: flex;
  gap: 30px;
  margin: 0;
}

.nav-links li a {
  color: rgb(0, 0, 0);
  text-decoration: none;
  font-size: 1rem;
  transition: 0.3s ease;
  padding: 5px 10px;
  border-radius: 5px;
}

/* Hover bonito */
.nav-links li a:hover {
  background: white;
  color: #2563eb;
}
</style>