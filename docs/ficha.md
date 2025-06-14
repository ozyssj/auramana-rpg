<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Ficha de Personagem - Auramana T20</title>
  <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&display=swap" rel="stylesheet">
  <style>
    :root {
      --cor-primaria: #5b4636;
      --cor-secundaria: #3a2c1d;
      --cor-fundo: #fdfaf3;
      --cor-texto: #3a2c1d;
      --cor-destaque: #bba88c;
    }

    body {
      background-color: #e8dbc3;
      font-family: 'MedievalSharp', cursive;
      padding: 20px;
      margin: 0;
      color: var(--cor-texto);
    }

    .ficha-container {
      background-color: var(--cor-fundo);
      border: 8px solid var(--cor-primaria);
      border-radius: 12px;
      max-width: 900px;
      margin: auto;
      padding: 20px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
    }

    h1, h2 {
      text-align: center;
      color: var(--cor-texto);
      text-shadow: 1px 1px var(--cor-destaque);
    }

    h1 { font-size: 2.2em; margin-bottom: 20px; }
    h2 { font-size: 1.5em; margin: 15px 0; }

    .campo {
      margin-bottom: 12px;
    }

    label {
      font-weight: bold;
      display: block;
      margin-bottom: 3px;
    }

    input, select, textarea, button {
      font-family: 'MedievalSharp', cursive;
      border: 2px solid var(--cor-primaria);
      border-radius: 5px;
      background-color: #fffaf0;
    }

    input, select, textarea {
      width: 100%;
      padding: 8px;
      font-size: 0.95em;
      box-shadow: inset 1px 1px 3px #ccc;
    }

    textarea {
      min-height: 80px;
      resize: vertical;
    }

    .atributos {
      display: grid;
      grid-template-columns: repeat(6, 1fr);
      gap: 12px;
      margin: 15px 0;
    }

    .linha {
      display: flex;
      gap: 15px;
    }

    .linha > * {
      flex: 1;
    }

    .botoes {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 10px;
      margin-top: 20px;
    }

    button {
      font-size: 1em;
      background-color: var(--cor-primaria);
      color: #fff9e6;
      padding: 8px 15px;
      cursor: pointer;
      box-shadow: 0 3px var(--cor-secundaria);
      transition: all 0.2s;
    }

    button:hover {
      background-color: var(--cor-secundaria);
    }

    button:active {
      transform: translateY(2px);
      box-shadow: 0 1px var(--cor-secundaria);
    }

    .pericias {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 12px;
    }
    
    .pericia {
      font-size: 0.85em;
      margin-bottom: 6px;
    }
    
    .pericia label {
      font-size: 0.9em;
    }
    
    .pericia input,
    .pericia select {
      padding: 5px;
      font-size: 0.85em;
    }

    .defesa {
      font-size: 1.3em;
      margin: 10px 0;
    }

    #uploadFicha {
      display: none;
    }

    @media (max-width: 768px) {
      .atributos, .pericias {
        grid-template-columns: repeat(2, 1fr);
      }
      
      .linha {
        flex-direction: column;
        gap: 10px;
      }
    }
  </style>
</head>
<body>
  <div class="ficha-container">
    <h1>Ficha Auramana T20</h1>

    <!-- Seção de Informações Básicas -->
    <div class="campo">
      <label for="nome">Nome</label>
      <input type="text" id="nome" placeholder="Ex: Lendor, o Errante">
    </div>

    <div class="linha">
      <div class="campo">
        <label for="nivel">Nível</label>
        <input type="number" id="nivel" min="0" max="60">
      </div>
      <div class="campo">
        <label for="xp">XP</label>
        <input type="number" id="xp">
      </div>
    </div>

    <div class="linha">
      <div class="campo">
        <label for="raca">Raça</label>
        <select id="raca">
          <option value="">-- Selecione --</option>
          <option>Humano</option>
          <option>Elfo</option>
          <option>Anão</option>
          <option>Goblinoide</option>
          <option>Gigante</option>
          <option>Pequenino</option>
          <option>Troll</option>
          <option>Morto-Vivo</option>        
          <option>Golem</option>
          <option>Feral</option>
          <option>Extraplanar</option>
        </select>
      </div>
      
      <div class="campo">
        <label for="classe">Classe</label>
        <select id="classe" onchange="filtrarArquetipos()">
          <option value="">-- Selecione --</option>
          <option value="Arcanista">Arcanista</option>
          <option value="Batedor">Batedor</option>
          <option value="Elementalista">Elementalista</option>
          <option value="Guerreiro">Guerreiro</option>
          <option value="Inspirador">Inspirador</option>
          <option value="Inventor">Inventor</option>
          <option value="Sacerdote">Sacerdote</option>
        </select>
      </div>
      
      <div class="campo">
        <label for="arquetipo">Arquétipo</label>
        <select id="arquetipo">
          <option value="">-- Selecione --</option>
        </select>
      </div>
    </div>

    <div class="linha">
      <div class="campo">
        <label for="origem">Origem</label>
        <input type="text" id="origem" placeholder="Ex: Eremita">
      </div>
      
      <div class="campo">
        <label for="divindade">Divindade</label>
        <input type="text" id="divindade" placeholder="Ex: São Nikolai">
      </div>
    </div>

    <!-- Seção de Atributos -->
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
        <label for="sab">SAB</label>
        <input type="number" id="sab" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="car">CAR</label>
        <input type="number" id="car" min="-10" max="10">
      </div>
    </div>

    <!-- Seção de PV/PM -->
    <div class="linha">
      <div class="campo">
        <label for="pvAtual">PV Atual</label>
        <input type="number" id="pvAtual">
      </div>
      <div class="campo">
        <label for="pvMax">PV Máx</label>
        <input type="number" id="pvMax">
      </div>
      <div class="campo">
        <label for="pvTemp">PV Temp</label>
        <input type="number" id="pvTemp">
      </div>
    </div>

    <div class="linha">
      <div class="campo">
        <label for="pmAtual">PM Atual</label>
        <input type="number" id="pmAtual">
      </div>
      <div class="campo">
        <label for="pmMax">PM Máx</label>
        <input type="number" id="pmMax">          
      </div>
      <div class="campo">
        <label for="pmTemp">PM Temp</label>
        <input type="number" id="pmTemp">          
      </div>
    </div>

    <!-- Seção de Defesa e Características -->
    <h2>Defesa</h2>
    <div class="defesa">
      <div class="linha">
        <div class="campo">
          <select class="atributo-pericia">
            <option value="des">DES</option>
            <option value="for">FOR</option>
            <option value="con">CON</option>
            <option value="int">INT</option>
            <option value="sab">SAB</option>
            <option value="car">CAR</option>
          </select>
          <select class="treinamento-pericia">
            <option value="10">Destreinado</option>
            <option value="12">Iniciante</option>
            <option value="14">Veterano</option>
            <option value="16">Mestre</option>
          </select>
          <input type="number" class="bonus-pericia" placeholder="Bônus">
          <input type="number" class="valor-pericia" readonly>
        </div>
      </div>
    </div>

    <div class="linha">
      <div class="campo">
        <label for="armadura">Armadura</label>
        <input type="text" id="armadura" placeholder="RD e Penalidade">
      </div>
      <div class="campo">
        <label for="deslocamento">Deslocamento</label>
        <input type="number" id="deslocamento" min="0" max="60" placeholder="9">
      </div>
      <div class="campo">
        <label for="tamanho">Tamanho</label>
        <select id="tamanho">
          <option>Médio</option>
          <option>Minúsculo</option>
          <option>Pequeno</option>
          <option>Grande</option>
          <option>Colossal</option>
        </select>
      </div>
    </div>

    <!-- Seção de Ataques -->
    <h2>Ataques</h2>
    <div class="campo">
      <textarea id="ataques" rows="4">
-> Espada Longa: 
- d20+8+2
- 1d8+4+3</textarea>
    </div>

    <!-- Seção de Perícias -->
    <h2>Perícias</h2>
    <div class="pericias" id="pericias-container"></div>




    <!-- Seção de Inventário e Poderes -->
    <div class="linha">
      <div class="campo">
        <label for="inventario">Inventário</label>
        <textarea id="inventario" rows="6">
-> Moedas: 
-> 
-> </textarea>
      </div>
      
      <div class="campo">
        <label for="poderes">Poderes</label>
        <textarea id="poderes" rows="6">
-> Raça: 
-> Origem: 
-> ND1: 
-> ND2: </textarea>
      </div>
    </div>

    <!-- Seção de Magias -->
    <h2>Magias</h2>
    <div class="campo">
      <textarea id="magias" rows="8">
-> 1° Círculo: 
- 
-
-> 2° Círculo: 
- 
- </textarea>
    </div>

    <!-- Botões de Ação -->
    <div class="botoes">
      <button onclick="salvarFicha()">Salvar</button>
      <button onclick="baixarFicha()">Exportar</button>
      <button onclick="document.getElementById('uploadFicha').click()">Importar</button>
      <button onclick="limparFicha()">Limpar</button>
      <input type="file" id="uploadFicha" accept=".json" onchange="carregarFicha()">
    </div>
  </div>

  <script>
    // Dados da aplicação
    const dados = {
      pericias: [
        { nome: "Acrobacia", atributo: "des" },
        { nome: "Adestramento", atributo: "car" },
        { nome: "Atletismo", atributo: "for" },
        { nome: "Atuação", atributo: "car" },
        { nome: "Cavalgar", atributo: "des" },
        { nome: "Conhecimento", atributo: "int" },
        { nome: "Cura", atributo: "sab" },
        { nome: "Diplomacia", atributo: "car" },
        { nome: "Enganação", atributo: "car" },
        { nome: "Fortitude", atributo: "con" },
        { nome: "Furtividade", atributo: "des" },
        { nome: "Guerra", atributo: "int" },
        { nome: "Iniciativa", atributo: "des" },
        { nome: "Intimidação", atributo: "car" },
        { nome: "Intuição", atributo: "sab" },
        { nome: "Investigação", atributo: "int" },
        { nome: "Jogatina", atributo: "car" },
        { nome: "Ladinagem", atributo: "des" },
        { nome: "Luta", atributo: "for" },
        { nome: "Misticismo", atributo: "int" },
        { nome: "Nobreza", atributo: "int" },
        { nome: "Ofício Alquimia", atributo: "int" },
        { nome: "Ofício Artilheiro", atributo: "int" },
        { nome: "Ofício Engenhoqueiro", atributo: "int" },
        { nome: "Ofício Ferreiro", atributo: "int" },
        { nome: "Ofício", atributo: "int" },
        { nome: "Percepção", atributo: "sab" },
        { nome: "Pilotagem", atributo: "des" },
        { nome: "Pontaria", atributo: "des" },
        { nome: "Reflexos", atributo: "des" },
        { nome: "Religião", atributo: "sab" },
        { nome: "Sobrevivência", atributo: "sab" },
        { nome: "Vontade", atributo: "sab" }
      ],
      
      atributos: [
        { value: "des", text: "DES" },
        { value: "for", text: "FOR" },
        { value: "con", text: "CON" },
        { value: "int", text: "INT" },
        { value: "sab", text: "SAB" },
        { value: "car", text: "CAR" }
      ],
      
      treinamentos: [
        { value: "0", text: "Destreinado" },
        { value: "2", text: "Iniciante" },
        { value: "4", text: "Veterano (ND7)" },
        { value: "6", text: "Mestre (ND13)" }
      ],
      
      arquetiposPorClasse: {
        Arcanista: ["Bruxo", "Feiticeiro", "Mago", "Necromante"],
        Batedor: ["Bucaneiro", "Caçador", "Duelista", "Investigador", "Ladino", "Ventanista"],
        Elementalista: ["Druida", "Místico", "Treinador"],
        Guerreiro: ["Bárbaro", "Cavaleiro", "Lutador", "Samurai", "Soldado"],
        Inspirador: ["Bardo", "Nobre", "Oráculo"],
        Inventor: ["Alquimista", "Artilheiro", "Ferreiro"],
        Sacerdote: ["Clérigo", "Frade", "Paladino", "Santo"]
      }
    };

    // Funções de inicialização
    function inicializarPericias() {
      const container = document.getElementById('pericias-container');
      container.innerHTML = dados.pericias
