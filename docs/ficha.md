<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Ficha de Personagem</title>
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

    input, select {
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

    .barra3colunas {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 15px;
    }

    .pericias {
      margin-top: 30px;
    }

    .pericia-item {
      display: flex;
      align-items: center;
      margin-bottom: 10px;
      gap: 10px;
    }

    .pericia-item select {
      width: auto;
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

    <div class="atributos">
      <div class="campo">
        <label for="for">FOR</label>
        <input type="number" id="for" min="-10" max="10">
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
        <input type="number" id="car" min="-10" max="10">
      </div>
    </div>

    <div class="barra3colunas">
      <div class="campo">
        <label for="pvMax">PV Máx</label>
        <input type="number" id="pvMax">
      </div>
      <div class="campo">
        <label for="pvTemp">PV Temporário</label>
        <input type="number" id="pvTemp">
      </div>
      <div class="campo">
        <label for="pvAtual">PV Atual</label>
        <input type="number" id="pvAtual">
      </div>
    </div>

    <div class="barra3colunas">
      <div class="campo">
        <label for="pmMax">PM Máx</label>
        <input type="number" id="pmMax">
      </div>
      <div class="campo">
        <label for="pmTemp">PM Temporário</label>
        <input type="number" id="pmTemp">
      </div>
      <div class="campo">
        <label for="pmAtual">PM Atual</label>
        <input type="number" id="pmAtual">
      </div>
    </div>

    <div class="campo">
      <label for="nivel">Nível</label>
      <input type="number" id="nivel" min="1" max="20">
    </div>

    <div class="pericias">
      <h2>Perícias</h2>
      <div id="lista-pericias"></div>
    </div>

    <div class="botoes">
      <button onclick="salvarFicha()">Salvar Ficha</button>
    </div>
  </div>

  <script>
    const pericias = [
      { nome: "Acrobacia", atributo: "des" },
      { nome: "Adestramento", atributo: "car" },
      { nome: "Arcanismo", atributo: "int" },
      { nome: "Atletismo", atributo: "for" },
      { nome: "Atuação", atributo: "car" },
      { nome: "Cavalgar", atributo: "des" },
      { nome: "Conhecimento", atributo: "int" },
      { nome: "Cura", atributo: "int" },
      { nome: "Diplomacia", atributo: "car" },
      { nome: "Enganação", atributo: "car" },
      { nome: "Fortitude", atributo: "con" },
      { nome: "Furtividade", atributo: "des" },
      { nome: "Guerra", atributo: "int" },
      { nome: "Intimidação", atributo: "car" },
      { nome: "Intuição", atributo: "sen" },
      { nome: "Investigação", atributo: "int" },
      { nome: "Jogatina", atributo: "car" },
      { nome: "Ladinagem", atributo: "des" },
      { nome: "Luta", atributo: "for" },
      { nome: "Misticismo", atributo: "int" },
      { nome: "Nobreza", atributo: "int" },
      { nome: "Ofício", atributo: "int" },
      { nome: "Percepção", atributo: "sen" },
      { nome: "Pilotagem", atributo: "des" },
      { nome: "Reflexos", atributo: "des" },
      { nome: "Religião", atributo: "sen" },
      { nome: "Sobrevivência", atributo: "sen" },
      { nome: "Vontade", atributo: "sen" }
    ];

    function criarListaPericias() {
      const container = document.getElementById("lista-pericias");
      container.innerHTML = "";
      pericias.forEach((p, i) => {
        const div = document.createElement("div");
        div.className = "pericia-item";
        div.innerHTML = `
          <label>${p.nome}</label>
          <select id="treinamento-${i}">
            <option value="0">Destreinado</option>
            <option value="2">Treinado</option>
            <option value="4">Veterano</option>
            <option value="6">Mestre</option>
          </select>
          <span id="valor-pericia-${i}">0</span>
        `;
        container.appendChild(div);
      });
    }

    function atualizarPericias() {
      const nivel = parseInt(document.getElementById("nivel").value || "0");
      pericias.forEach((p, i) => {
        const atr = parseInt(document.getElementById(p.atributo).value || "0");
        const grau = parseInt(document.getElementById(`treinamento-${i}`).value || "0");
        const valor = Math.floor(nivel / 2) + atr + grau;
        document.getElementById(`valor-pericia-${i}`).textContent = valor;
      });
    }

    function salvarFicha() {
      const campos = ['nome', 'raca', 'origem', 'nivel', 'for', 'des', 'con', 'int', 'sen', 'car', 'pvMax', 'pvTemp', 'pvAtual', 'pmMax', 'pmTemp', 'pmAtual'];
      campos.forEach(id => {
        const valor = document.getElementById(id).value;
        localStorage.setItem('ficha-' + id, valor);
      });
      pericias.forEach((p, i) => {
        const val = document.getElementById(`treinamento-${i}`).value;
        localStorage.setItem(`ficha-pericia-${i}`, val);
      });
      alert("Ficha salva nas memórias do grimório!");
    }

    window.onload = () => {
      const campos = ['nome', 'raca', 'origem', 'nivel', 'for', 'des', 'con', 'int', 'sen', 'car', 'pvMax', 'pvTemp', 'pvAtual', 'pmMax', 'pmTemp', 'pmAtual'];
      campos.forEach(id => {
        const valor = localStorage.getItem('ficha-' + id);
        if (valor) document.getElementById(id).value = valor;
      });
      criarListaPericias();
      pericias.forEach((p, i) => {
        const val = localStorage.getItem(`ficha-pericia-${i}`);
        if (val) document.getElementById(`treinamento-${i}`).value = val;
      });
      document.querySelectorAll('input, select').forEach(el => el.addEventListener('input', atualizarPericias));
      atualizarPericias();
    };
  </script>
</body>
</html>
