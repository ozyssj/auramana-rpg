<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Ficha de Personagem - Tormenta20</title>
  <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #e8dbc3;
      font-family: 'MedievalSharp', cursive;
      padding: 30px;
      margin: 0;
    }

    .ficha-container {
      background-color: #fdfaf3;
      border: 8px solid #5b4636;
      border-radius: 12px;
      max-width: 900px;
      margin: auto;
      padding: 30px;
      box-shadow: 0 0 30px rgba(0, 0, 0, 0.3);
    }

    h1 {
      text-align: center;
      font-size: 2.5em;
      margin-bottom: 30px;
      color: #3a2c1d;
      text-shadow: 1px 1px #bba88c;
    }

    .campo {
      margin-bottom: 15px;
    }

    label {
      font-weight: bold;
      display: block;
      font-size: 1.2em;
      margin-bottom: 4px;
    }

    input, select, textarea {
      width: 100%;
      padding: 10px;
      font-family: 'MedievalSharp', cursive;
      font-size: 1em;
      border: 2px solid #5b4636;
      border-radius: 5px;
      background-color: #fffaf0;
      box-shadow: inset 1px 1px 3px #ccc;
    }

    .atributos {
      display: grid;
      grid-template-columns: repeat(6, 1fr);
      gap: 15px;
      margin-top: 20px;
    }

    .botoes {
      text-align: center;
      margin-top: 30px;
    }

    button {
      font-family: 'MedievalSharp', cursive;
      font-size: 1.2em;
      background-color: #5b4636;
      color: #fff9e6;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      cursor: pointer;
      box-shadow: 0 4px #3a2c1d;
    }

    button:hover {
      background-color: #3a2c1d;
    }

    button:active {
      transform: translateY(2px);
      box-shadow: 0 2px #3a2c1d;
    }
  </style>
</head>
<body>

  <div class="ficha-container">
    <h1>Ficha de Personagem</h1>

    <div class="campo">
      <label for="nome">Nome</label>
      <input type="text" id="nome" placeholder="Ex: Lendor, o Errante">
    </div>

    <div class="campo">
      <label for="raca">Raça</label>
      <select id="raca">
        <option value="">-- Selecione a Raça --</option>
        <option value="Humano">Humano</option>
        <option value="Elfo">Elfo</option>
        <option value="Anão">Anão</option>
        <option value="Orc">Goblinoide</option>
        <option value="Goblin">Troll</option>
        <option value="Meio-Elfo">Feral</option>
        <option value="Tiefling">Extraplanar</option>
        <option value="Draconato">Gigante</option>
      </select>
    </div>

    <div class="campo">
      <label for="origem">Origem</label>
      <input type="text" id="origem" placeholder="Ex: Eremita">
    </div>

    <div class="campo">
      <label for="classe">Classe</label>
      <input type="text" id="classe" placeholder="Ex: Guerreiro">
    </div>

    <div class="campo">
      <label for="nivel">Nível</label>
      <input type="number" id="nivel" min="1" max="20">
    </div>

    <div class="campo">
      <label for="pv">Pontos de Vida (PV)</label>
      <input type="number" id="pv" min="0">
    </div>

    <div class="campo">
      <label for="pm">Pontos de Mana (PM)</label>
      <input type="number" id="pm" min="0">
    </div>

    <div class="campo">
      <label for="defesa">Defesa</label>
      <input type="number" id="defesa" min="0">
    </div>

    <div class="campo">
      <label for="deslocamento">Deslocamento</label>
      <input type="text" id="deslocamento" placeholder="Ex: 9m">
    </div>

    <div class="atributos">
      <div class="campo">
        <label for="for">FOR</label>
        <input type="number" id="for"  min="-10" max="10">
      </div>
      <div class="campo">
        <label for="des">DES</label>
        <input type="number" id="des" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="con">CON</label>
        <input type="number" id="con" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="int">INT</label>
        <input type="number" id="int" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="sen">SEN</label>
        <input type="number" id="sen" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="car">CAR</label>
        <input type="number" id="car"  min="-10" max="10">
      </div>
    </div>

    <div class="campo">
      <label for="poderes">Poderes</label>
      <textarea id="poderes" rows="4" placeholder="Descreva aqui os poderes especiais e habilidades."></textarea>
    </div>

    <div class="campo">
      <label for="equipamentos">Equipamentos</label>
      <textarea id="equipamentos" rows="4" placeholder="Liste os itens e armas que carrega."></textarea>
    </div>

    <div class="botoes">
      <button onclick="salvarFicha()">Salvar Ficha</button>
    </div>
  </div>

  <script>
    function salvarFicha() {
      const campos = ['nome', 'raca', 'origem', 'classe', 'nivel', 'pv', 'pm', 'defesa', 'deslocamento', 'for', 'des', 'con', 'int', 'sen', 'car', 'poderes', 'equipamentos'];
      campos.forEach(id => {
        const valor = document.getElementById(id).value;
        localStorage.setItem('ficha-' + id, valor);
      });
      alert("Ficha salva nas memórias do grimório (localStorage)!");
    }

    window.onload = () => {
      const campos = ['nome', 'raca', 'origem', 'classe', 'nivel', 'pv', 'pm', 'defesa', 'deslocamento', 'for', 'des', 'con', 'int', 'sen', 'car', 'poderes', 'equipamentos'];
      campos.forEach(id => {
        const valor = localStorage.getItem('ficha-' + id);
        if (valor) {
          document.getElementById(id).value = valor;
        }
      });
    }
  </script>

</body>
</html>
