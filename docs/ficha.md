<input type="text" id="nome" placeholder="Nome do personagem">
<button onclick="salvarFicha()">Salvar</button>
<script>
function salvarFicha() {
  const nome = document.getElementById('nome').value;
  localStorage.setItem('ficha-nome', nome);
}

window.onload = () => {
  const nome = localStorage.getItem('ficha-nome');
  if (nome) {
    document.getElementById('nome').value = nome;
  }
}
</script>
