<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Ficha de Personagem - Auramana T20</title>
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

    .linha {
      display: flex;
      gap: 20px;
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

    .pericias {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }
    
    .pericia {
        font-size: 0.8em;
        margin-bottom: 8px;
    }
    
    .pericia label {
        font-size: 0.9em;
        margin-bottom: 2px;
    }
    
    .pericia input,
    .pericia select {
        padding: 6px;
        font-size: 0.9em;
    }

    .defesa {
        font-size: 1.5em;
        margin-bottom: 8px;
    }        
        
  </style>
</head>
<body>
  <div class="ficha-container">
    <h1>Ficha Auramana T20</h1>

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

    <div class="campo">
      <label for="raca">Raça</label>
      <select id="raca">
        <option value="">-- Selecione a Raça --</option>
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
      <option value="">-- Selecione a Classe --</option>
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
        <option value="">-- Selecione o Arquétipo --</option>
    </select>
  </div>

    <div class="campo">
      <label for="origem">Origem</label>
      <input type="text" id="origem" placeholder="Ex: Eremita">
    </div>
    
    <div class="campo">
      <label for="origem">Divindade</label>
      <input type="text" id="origem" placeholder="Ex: São Nikolai">
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
        <label for="sab">SAB</label>
        <input type="number" id="sab" min="-10" max="10">
      </div>
      <div class="campo">
        <label for="car">CAR</label>
        <input type="number" id="car" min="-10" max="10">
      </div>
    </div>

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

    <div class="campo">
      <label for="armadura">Armadura </label>
      <input type="text" id="armadura" placeholder="RD e Penalidade">
    </div>

    <div class="linha">
     <div class="campo">
       <label for="deslocamento">Deslocamento </label>
       <input type="number" id="deslocamento" min="0" max="60" placeholder=9>
     </div>
    <div class="campo">
      <label for="classe">Tamanho</label>
      <select id="classe">
        <option>Médio</option>
        <option>Minúsculo</option>
        <option>Pequeno</option>
        <option>Grande</option>
        <option>Colossal</option>
      </select>
    </div>
    </div>
    
 <div class="pericia">
 <div class="defesa">
    <div class="linha">
      <div class="campo">
        <label>Defesa</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="10">Destreinado em Reflexos</option>
          <option value="12">Iniciante</option>
          <option value="14">Veterano (ND7)</option>
          <option value="16">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Defesa">
        <input type="number" class="valor-pericia" readonly>
      </div>
    </div>
</div>
</div>
    <div class="linha">
    <div class="campo">
        
<div class="campo">
  <label for="ataques">Ataques</label>
  <textarea id="ataques" rows="6">
 -> Espada Longa: 
 - d20+8+2
 - 1d8+4+3
</textarea>
</div>

    <h2>Perícias</h2>
    
 <div class="pericias" id="pericias-container">
</div>

<script>
  const pericias = [
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
  ];

  // Opções de atributos
  const atributos = [
    { value: "des", text: "DES" },
    { value: "for", text: "FOR" },
    { value: "con", text: "CON" },
    { value: "int", text: "INT" },
    { value: "sab", text: "SAB" },
    { value: "car", text: "CAR" }
  ];

  // Opções de treinamento
  const treinamentos = [
    { value: "0", text: "Destreinado" },
    { value: "2", text: "Iniciante" },
    { value: "4", text: "Veterano (ND7)" },
    { value: "6", text: "Mestre (ND13)" }
  ];

  // Função para gerar o HTML de uma perícia
  function criarPericia(pericia) {
    return `
      <div class="pericia">
        <label>${pericia.nome}</label>
        <select class="atributo-pericia">
          ${atributos.map(a => 
            `<option value="${a.value}" ${a.value === pericia.atributo ? 'selected' : ''}>${a.text}</option>`
          ).join('')}
        </select>
        <select class="treinamento-pericia">
          ${treinamentos.map(t => 
            `<option value="${t.value}">${t.text}</option>`
          ).join('')}
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
    `;
  }

  // Gerar todas as perícias
  document.getElementById('pericias-container').innerHTML = pericias.map(criarPericia).join('');
</script>

<div class="campo">
  <label for="inventario">Inventário</label>
  <textarea id="inventario" rows="6">
 -> Moedas: 
 -> 
 -> 
</textarea>
</div>


<div class="campo">
  <label for="poderes">Poderes</label>
  <textarea id="poderes" rows="22">
 -> Raça: 
 -> Origem: 
 -> ND1: 
 -> ND2: 
 -> ND3: 
 -> ND4: 
 -> ND5: 
</textarea>
</div>

<div class="campo">
  <label for="magias">Magias</label>
  <textarea id="magias" rows="20">
 -> 1° Círculo: 
 - 
 -
 -> 2° Círculo: 
 - 
 - 
 -> 3° Círculo: 
 - 
</textarea>
</div>


<div class="botoes">
  <button onclick="salvarFicha()">Salvar no Navegador</button>
  <button onclick="baixarFicha()">Exportar Ficha</button>
  <input type="file" id="uploadFicha" accept=".json" onchange="carregarFicha()" style="display:none">
  <button onclick="document.getElementById('uploadFicha').click()">Importar Ficha</button>
    <button onclick="limparFicha()">Limpar Ficha</button>

</div>

  </div>




<script>
function atualizarPericias() {
  const nivel = parseInt(document.getElementById('nivel').value) || 0;
  const atributos = {
    for: parseInt(document.getElementById('for').value) || 0,
    des: parseInt(document.getElementById('des').value) || 0,
    con: parseInt(document.getElementById('con').value) || 0,
    int: parseInt(document.getElementById('int').value) || 0,
    sab: parseInt(document.getElementById('sab').value) || 0,
    car: parseInt(document.getElementById('car').value) || 0
  };

  document.querySelectorAll('.pericia').forEach(div => {
    const atributo = div.querySelector('.atributo-pericia').value;
    const treinamento = parseInt(div.querySelector('.treinamento-pericia').value);
    const bonusAdicional = parseInt(div.querySelector('.bonus-pericia').value) || 0;
    const valor = Math.floor(nivel / 2) + atributos[atributo] + treinamento + bonusAdicional;
    div.querySelector('.valor-pericia').value = valor;
  });
}

['nivel', 'for', 'des', 'con', 'int', 'sab', 'car'].forEach(id => {
  document.getElementById(id).addEventListener('input', atualizarPericias);
});

document.addEventListener('change', e => {
  if (e.target.classList.contains('atributo-pericia') || e.target.classList.contains('treinamento-pericia') || e.target.classList.contains('bonus-pericia')) {
    atualizarPericias();
  }
});

function salvarFicha() {
  const campos = document.querySelectorAll('input, select, textarea');
  campos.forEach(el => localStorage.setItem('ficha-' + el.id, el.value));
  alert("Ficha salva nas memórias do grimório!");
}

function baixarFicha() {
  const campos = document.querySelectorAll('input, select, textarea');
  const ficha = {};
  campos.forEach(el => {
    ficha[el.id] = (el.type === 'checkbox') ? el.checked : el.value;
  });

  const blob = new Blob([JSON.stringify(ficha, null, 2)], { type: 'application/json' });
  const url = URL.createObjectURL(blob);

  const a = document.createElement('a');
  a.href = url;
  const nome = document.getElementById('nome').value;
  a.download = nome + '_ficha_t20.json';
  a.click();

  URL.revokeObjectURL(url);
}

function carregarFicha() {
  const input = document.getElementById('uploadFicha');
  const file = input.files[0];
  if (!file) return;

  const reader = new FileReader();
  reader.onload = function (e) {
    const data = JSON.parse(e.target.result);
    Object.keys(data).forEach(id => {
      const el = document.getElementById(id);
      if (el) {
        if (el.type === 'checkbox') {
          el.checked = data[id];
        } else {
          el.value = data[id];
        }
        localStorage.setItem('ficha-' + id, data[id]);
      }
    });
    alert("Ficha carregada com sucesso!");
  };
  reader.readAsText(file);
}

function limparFicha() {
  if (confirm("Tem certeza que deseja apagar todos os dados da ficha?")) {
    const campos = document.querySelectorAll('input, select, textarea');
    campos.forEach(el => {
      localStorage.removeItem('ficha-' + el.id);
      if (el.type === 'checkbox') {
        el.checked = false;
      } else if (el.tagName === 'SELECT') {
        el.selectedIndex = 0;
      } else {
        el.value = '';
      }
    });
    document.getElementById('output-json').value = '';
    alert("Todos os dados foram apagados da ficha.");
  }
}


const arquetiposPorClasse = {
  Arcanista: ["Bruxo", "Feiticeiro", "Mago", "Necromante"],
  Batedor: ["Bucaneiro", "Caçador", "Duelista", "Investigador", "Ladino", "Ventanista"],
  Elementalista: ["Druida", "Místico", "Treinador"],
  Guerreiro: ["Bárbaro", "Cavaleiro", "Lutador", "Samurai", "Soldado"],
  Inspirador: ["Bardo", "Nobre", "Oráculo"],
  Inventor: ["Alquimista", "Artilheiro", "Ferreiro"],
  Sacerdote: ["Clérigo", "Frade", "Paladino", "Santo"]
};

function filtrarArquetipos() {
  const classe = document.getElementById("classe").value;
  const arquetipoSelect = document.getElementById("arquetipo");

  // Limpa os arquétipos atuais
  arquetipoSelect.innerHTML = '<option value="">-- Selecione o Arquétipo --</option>';

  if (arquetiposPorClasse[classe]) {
    arquetiposPorClasse[classe].forEach(arq => {
      const option = document.createElement("option");
      option.text = arq;
      option.value = arq;
      arquetipoSelect.add(option);
    });
  }
}


window.onload = () => {
  const campos = document.querySelectorAll('input, select, textarea');
  campos.forEach(el => {
    const val = localStorage.getItem('ficha-' + el.id);
    if (val) el.value = val;
  });
  atualizarPericias();
};

</script>
</body>
</html>
