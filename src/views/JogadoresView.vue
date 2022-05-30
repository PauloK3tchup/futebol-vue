<script>
import ListaTimes from "@/components/ListaTimes.vue";
export default {
  mounted() {
    const checkbox = document.getElementById("mostrar-times");
    const box = document.getElementById("times");
    checkbox.addEventListener("click", function handleClick() {
      if (checkbox.checked) {
        box.style.display = "block";
      } else {
        box.style.display = "none";
      }
    });
  },
  components: { ListaTimes },
};
</script>
<template>
  <h1>Cadastrar Jogadores:</h1>
  <form action="">
    <input placeholder="Nome do Jogador" type="text" id="nome-jogador" />
    <select name="Função" id="Funções">
      <option id="gol" value="Goleiro">Goleiro</option>
      <option id="zag" value="Zagueiro">Zagueiro</option>
      <option id="lib" value="Líbero">Líbero</option>
      <option id="ata" value="Atacante">Atacante</option>
      <option id="vol" value="Volante">Volante</option>
      <option id="ala" value="Ala">Ala</option>
      <option id="lat" value="Lateral">Lateral</option>
    </select>
    <br />
    <button class="Enviar">Enviar</button>
    <div class="checkbox-times">
      <input type="checkbox" name="Mostrar" id="mostrar-times" />
      <label for="mostrar-times">Mostrar Times</label>
    </div>
    <div id="times">
      <ListaTimes />
    </div>
  </form>
</template>

<style></style>
