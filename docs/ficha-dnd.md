<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <title>Ficha de Personagem - T20</title>
  <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&display=swap" rel="stylesheet">
  <style>
    :root {
      --cor-primaria: #36475b;
      --cor-secundaria: #2c1d3a;
      --cor-fundo: #c8c8db;
      --cor-texto: #281d3a;
      --cor-destaque: #8e8cbb;
    }

    body {
      background-color: #c3c3e8;
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

    h1,
    h2 {
      text-align: center;
      color: var(--cor-texto);
      text-shadow: 1px 1px var(--cor-destaque);
    }

    h1 {
      font-size: 2.2em;
      margin-bottom: 20px;
    }

    h2 {
      font-size: 1.5em;
      margin: 15px 0;
    }

    .campo {
      margin-bottom: 12px;
    }

    label {
      font-weight: bold;
      display: block;
      margin-bottom: 3px;
    }

    input,
    select,
    textarea,
    button {
      font-family: 'MedievalSharp', cursive;
      border: 2px solid var(--cor-primaria);
      border-radius: 5px;
      background-color: #fffaf0;
    }

    input,
    select,
    textarea {
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

    .linha>* {
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
      grid-template-columns: repeat(3, minmax(0, 1fr));
      /* Força 3 colunas */
      gap: 15px;
      width: 100%;
      overflow: hidden;
      /* Evita problemas de overflow */
    }

    .pericia {
      min-width: 0;
      /* Corrige problemas de flexibilidade */
      break-inside: avoid;
      /* Evita quebras indesejadas */
      page-break-inside: avoid;
      /* Para compatibilidade */
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
      font-size: 1.0em;
      margin: 10px 0;
    }

    #uploadFicha {
      display: none;
    }

    @media (max-width: 768px) {

      .atributos,
      .pericias {
        grid-template-columns: repeat(3, 1fr);
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
    <h1>Ficha Auramana D&D</h1>

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
        <label for="xp">Bônus de Proficiência</label>
        <input type="number" id="proficiencia" readonly>
      </div>
      <div class="campo">
        <label for="xp">XP</label>
        <input type="number" id="xp">
      </div>
    </div>

    <div class="campo">
      <label for="raca">Raça</label>
      <input type="text" id="raca" placeholder="Ex: Goblin">
    </div>


    <div class="campo">
      <label for="classe">Classe</label>
      <select id="classe" onchange="calcularAtributos()">
        <option value="">-- Selecione a Classe --</option>
        <option value="ARTI">Artífice</option>
        <option value="BARB">Bárbaro</option>
        <option value="BARD">Bardo</option>
        <option value="BRUX">Bruxo</option>
        <option value="CLER">Clérigo</option>
        <option value="DRUI">Druida</option>
        <option value="FEIT">Feiticeiro</option>
        <option value="GUAR">Guardião</option>
        <option value="GUER">Guerreiro</option>
        <option value="LADI">Ladino</option>
        <option value="MAGO">Mago</option>
        <option value="MONG">Monge</option>
        <option value="PALA">Paladino</option>
      </select>
    </div>



    <div class="campo">
      <label for="origem">Origem</label>
      <input type="text" id="origem" placeholder="Ex: Eremita">
    </div>

    <div class="campo">
      <label for="origem">Divindade</label>
      <input type="text" id="origem" placeholder="Ex: Valkaria">
    </div>

    <div class="atributos">
      <div class="campo">
        <label for="for">FOR</label>
        <input type="number" id="for" min="-5" max="10">
      </div>
      <div class="campo">
        <label for="des">DES</label>
        <input type="number" id="des" min="-5" max="10">
      </div>
      <div class="campo">
        <label for="con">CON</label>
        <input type="number" id="con" min="-5" max="10">
      </div>
      <div class="campo">
        <label for="int">INT</label>
        <input type="number" id="int" min="-5" max="10">
      </div>
      <div class="campo">
        <label for="sab">SAB</label>
        <input type="number" id="sab" min="-5" max="10">
      </div>
      <div class="campo">
        <label for="car">CAR</label>
        <input type="number" id="car" min="-5" max="10">
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

    <div class="linha">
      <div class="campo">
        <label for="armadura">Armadura: </label>
        <input type="text" id="armadura" placeholder="Leve ou Pesada">
      </div>

      <div class="campo">
        <label for="armadura">Defesa</label>
        <input type="number" id="defesa" placeholder=10>
      </div>
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

    <div class="campo">
      <label for="origem">Proficiências</label>
      <input type="text" id="proficiencia" placeholder="Ex: Armas marciais, ferramentas de alquimista.">
    </div>

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
        { nome: "Salvaguarda FOR", atributo: "for" },
        { nome: "Salvaguarda DES", atributo: "des" },
        { nome: "Salvaguarda CON", atributo: "con" },
        { nome: "Salvaguarda INT", atributo: "int" },
        { nome: "Salvaguarda SAB", atributo: "sab" },
        { nome: "Salvaguarda CAR", atributo: "car" },        
        { nome: "Acrobacia", atributo: "des" },
        { nome: "Arcanismo", atributo: "car" },
        { nome: "Atletismo", atributo: "for" },
        { nome: "Atuação", atributo: "car" },
        { nome: "Enganação", atributo: "car" },
        { nome: "Furtividade", atributo: "des" },
        { nome: "História", atributo: "int" },
        { nome: "Intimidação", atributo: "car" },
        { nome: "Intuição", atributo: "sab" },
        { nome: "Investigação", atributo: "int" },
        { nome: "Iniciativa", atributo: "des" },
        { nome: "Ladinagem", atributo: "des" },
        { nome: "Lidar Com Animais", atributo: "car" },
        { nome: "Medicina", atributo: "sab" },
        { nome: "Natureza", atributo: "int" },
        { nome: "Persuasão", atributo: "car" },
        { nome: "Percepção", atributo: "sab" },
        { nome: "Religião", atributo: "int" },
        { nome: "Sobrevivência", atributo: "sab" },
        { nome: "Cavalgar", atributo: "des" },
        { nome: "Estratégia", atributo: "int" },
        { nome: "Ferramenta", atributo: "int" },
        { nome: "Ofício", atributo: "int" },
        { nome: "Pilotagem", atributo: "des" }

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
        { value: "1", text: "Treinado" },
        { value: "2", text: "Especialista" }
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
        const bonusProficiencia = parseInt(document.getElementById('proficiencia').value) || 0;
        const bonusAdicional = parseInt(div.querySelector('.bonus-pericia').value) || 0;
        const valor = atributos[atributo] + (treinamento * bonusProficiencia) + bonusAdicional;
        div.querySelector('.valor-pericia').value = valor;
      });

      document.querySelectorAll('.defesa').forEach(div => {
        const atributo = div.querySelector('.atributo-pericia').value;
        const treinamento = parseInt(div.querySelector('.treinamento-pericia').value);
        const bonusProficiencia = parseInt(document.getElementById('proficiencia').value) || 0;
        const bonusAdicional = parseInt(div.querySelector('.bonus-pericia').value) || 0;
        const valor = atributos[atributo] + (treinamento * bonusProficiencia) + bonusAdicional;
        div.querySelector('.valor-defesa').value = 10 + valor;
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


    // Constantes com os valores base por classe
    const BASES_PV = {
      'ARTI': 5,
      'BARB': 7,
      'BARD': 5,
      'BRUX': 5,
      'CLER': 5,
      'DRUI': 5,
      'FEIT': 4,
      'GUAR': 6,
      'GUER': 6,
      'LADI': 5,
      'MAGO': 4,
      'MONG': 5,
      'PALA': 6,
    };

    const BASES_PM = {
      'ARTI': 5,
      'BARB': 1,
      'BARD': 5,
      'BRUX': 3,
      'CLER': 5,
      'DRUI': 5,
      'FEIT': 5,
      'GUAR': 4,
      'GUER': 3,
      'LADI': 3,
      'MAGO': 5,
      'MONG': 4,
      'PALA': 4,
    };


    function calcularAtributos() {

      calcularProficiencia();

      const constituicao = parseInt(document.getElementById('con').value) || 0;
      const nivel = parseInt(document.getElementById('nivel').value) || 1;
      const classe = document.getElementById('classe').value;

      // Cálculo de PV
      if (classe && BASES_PV[classe]) {
        const basePV = BASES_PV[classe];
        const pvInicial = (2 * basePV) - 2;
        const pvInicialExtra = pvInicial - basePV;
        const pvMax = ((basePV + constituicao) * nivel) + pvInicialExtra;
        document.getElementById('pvMax').value = pvMax;

        // Ajustar PV atual se necessário
        const pvAtual = parseInt(document.getElementById('pvAtual').value) || 0;
        if (pvAtual > pvMax || isNaN(pvAtual)) {
          document.getElementById('pvAtual').value = pvMax;
        }
      }

      // Cálculo de PM
      if (classe && BASES_PM[classe]) {
        const basePM = BASES_PM[classe];
        const pmMax = (basePM * nivel);
        document.getElementById('pmMax').value = pmMax;

        // Ajustar PM atual se necessário
        const pmAtual = parseInt(document.getElementById('pmAtual').value) || 0;
        if (pmAtual > pmMax || isNaN(pmAtual)) {
          document.getElementById('pmAtual').value = pmMax;
        }
      }

    }

    function calcularProficiencia() {
      const nivel = parseInt(document.getElementById('nivel').value) || 0;
      let proficiencia;

      if (nivel >= 1 && nivel <= 4) {
        proficiencia = 2;
      } else if (nivel >= 5 && nivel <= 8) {
        proficiencia = 3;
      } else if (nivel >= 9 && nivel <= 12) {
        proficiencia = 4;
      } else if (nivel >= 13 && nivel <= 16) {
        proficiencia = 5;
      } else if (nivel >= 17 && nivel <= 20) {
        proficiencia = 6;
      } else {
        proficiencia = 0; // Para níveis fora do intervalo 1-20
      }

      document.getElementById('proficiencia').value = proficiencia;
    }


    // Função auxiliar para ajustar valores atuais
    function ajustarValorAtual(idElemento, valorMax) {
      const elemento = document.getElementById(idElemento);
      if (!elemento.value || parseInt(elemento.value) > valorMax) {
        elemento.value = valorMax;
      }
    }

    // Configuração de eventos unificada
    function configurarEventos() {
      // Eventos que disparam o cálculo
      ['con', 'nivel', 'classe'].forEach(id => {
        document.getElementById(id).addEventListener('input', calcularAtributos);
      });

      // Listener específico para o nível (para atualizar perícias também)
      document.getElementById('nivel').addEventListener('input', function () {
        calcularAtributos();
        atualizarPericias();
      });

      // Validar valores atuais
      document.getElementById('pvAtual').addEventListener('change', function () {
        ajustarValorAtual('pvAtual', document.getElementById('pvMax').value);
      });

      document.getElementById('pmAtual').addEventListener('change', function () {
        ajustarValorAtual('pmAtual', document.getElementById('pmMax').value);
      });
    }

    // Inicialização completa
    window.addEventListener('DOMContentLoaded', () => {
      // Configurar eventos e calcular valores iniciais
      configurarEventos();
      calcularAtributos();
    });

    window.addEventListener('DOMContentLoaded', () => {
      // Carregar valores salvos
      const campos = document.querySelectorAll('input, select, textarea');
      campos.forEach(el => {
        const val = localStorage.getItem('ficha-' + el.id);
        if (val) el.value = val;
      });

      // Configurar eventos e calcular valores iniciais
      configurarEventos();
      calcularAtributos();
      atualizarPericias();
    });

    window.onload = () => {
      const campos = document.querySelectorAll('input, select, textarea');
      campos.forEach(el => {
        const val = localStorage.getItem('ficha-' + el.id);
        if (val) el.value = val;
      });
      configurarEventos();
      calcularAtributos();
      atualizarPericias();
    };

  </script>
</body>

</html>