<script setup></script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/categorias">Categoria</RouterLink>
      <RouterLink to="/temas">Tema</RouterLink>
      <RouterLink to="/produtos">Produto</RouterLink>
    </nav>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  height: 5rem;
}

nav {
  width: 100%;
  text-align: center;
  margin-top: 1rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  /* display: inline-block; */
  padding: 0 1rem;
  font-size: 1.5rem;
  text-decoration: none;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
