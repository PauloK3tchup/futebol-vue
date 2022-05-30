<script>
import ListaTimes from "@/components/ListaTimes.vue";
export default {
  components: { ListaTimes },
};
</script>
<template>
  <h1>Cadastrar Times:</h1>
  <form action="">
    <input placeholder="Nome do Time" type="text" id="nome-jogador" />
    <button class="Enviar">Enviar</button>
  </form>
  <ListaTimes />
</template>
<style></style>
