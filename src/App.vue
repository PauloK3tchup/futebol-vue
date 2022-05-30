<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/"><h3>Home</h3></RouterLink>
        <RouterLink to="/times"><h3>Times</h3></RouterLink>
        <RouterLink to="/jogadores"><h3>Jogadores</h3></RouterLink>
      </nav>
    </div>
  </header>
  <main class="content"><RouterView /></main>
  <footer><h3>Isso é um rodapé!</h3></footer>
</template>

<style></style>
