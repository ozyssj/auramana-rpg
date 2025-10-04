<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8" />
    <title>Ficha de Personagem - Auramana Pathfinder</title>
    <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&display=swap" rel="stylesheet">
    <style>
        /* --- (mantive seu CSS) --- */
        :root {
            --cor-primaria: #36475b;
            --cor-secundaria: #54acc4;
            --cor-fundo: #b8d4e1;
            --cor-texto: #281d3a;
            --cor-destaque: #54acc4;
        }

        body {
            background-color: #eff7f9;
            font-family: 'MedievalSharp', cursive;
            padding: 20px;
            margin: 0;
            color: var(--cor-texto)
        }

        .ficha-container {
            background-color: var(--cor-fundo);
            border: 8px solid var(--cor-primaria);
            border-radius: 12px;
            max-width: 1000px;
            margin: auto;
            padding: 20px;
            box-shadow: 0 0 20px rgba(0, 0, 0, .2)
        }

        h1,
        h2 {
            text-align: center;
            color: var(--cor-texto);
            text-shadow: 1px 1px var(--cor-destaque)
        }

        h1 {
            font-size: 2.2em;
            margin-bottom: 20px
        }

        h2 {
            font-size: 1.5em;
            margin: 15px 0
        }

        .campo {
            margin-bottom: 12px
        }

        .campo-atributo {
            text-align: center;
            margin-bottom: 10px
        }

        label {
            font-weight: bold;
            display: block;
            margin-bottom: 3px
        }

        input,
        select,
        textarea,
        button {
            font-family: 'MedievalSharp', cursive;
            border: 2px solid var(--cor-primaria);
            border-radius: 5px;
            background-color: #fffaf0
        }

        input,
        select,
        textarea {
            width: 100%;
            padding: 8px;
            font-size: .95em;
            box-shadow: inset 1px 1px 3px #ccc
        }

        input {
            text-align: center
        }

        textarea {
            min-height: 80px;
            resize: vertical
        }

        .atributos {
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            gap: 12px;
            margin: 15px 0
        }

        .duplo {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin: 15px 0
        }

        .triplo {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 12px;
            margin: 15px 0
        }

        .linha {
            display: flex;
            gap: 15px
        }

        .linha>* {
            flex: 1
        }

        .botoes {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 10px;
            margin-top: 20px
        }

        button {
            font-size: 1em;
            background-color: var(--cor-primaria);
            color: #fff9e6;
            padding: 8px 15px;
            cursor: pointer;
            box-shadow: 0 3px var(--cor-secundaria);
            transition: all .2s
        }

        button:hover {
            background-color: var(--cor-secundaria)
        }

        button:active {
            transform: translateY(2px);
            box-shadow: 0 1px var(--cor-secundaria)
        }

        .campo-pericia {
            width: 40%;
            text-align: right;
            padding-right: 10px
        }

        .campo-pericia2 {
            width: 25%;
            text-align: center
        }

        .campo-pericia3 {
            width: 15%;
            text-align: center
        }

        .campo-pericia4 {
            width: 50%;
            text-align: center
        }

        .campo-pericia5 {
            width: 30%;
            text-align: center
        }

        .linha-pericia {
            display: flex;
            flex: 1;
            font-size: .9em;
            margin: 0
        }

        .pericias {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 0;
            width: 100%;
            overflow: hidden
        }

        .pericia {
            min-width: 10px;
            break-inside: avoid;
            page-break-inside: avoid;
            font-size: .9em;
            margin-bottom: 0
        }

        .pericia label {
            font-size: 1.0em
        }

        .pericia input,
        .pericia select {
            text-align: center;
            padding: 0;
            font-size: .9em
        }

        @media (max-width:768px) {
            .atributos {
                grid-template-columns: repeat(3, 1fr)
            }

            .linha {
                flex-direction: column;
                gap: 10px
            }
        }
    </style>
</head>

<body>
    <div class="ficha-container">
        <h1>Ficha Auramana (PF2e)</h1>

        <div class="campo">
            <label for="nome">Nome</label>
            <input type="text" id="nome" placeholder="Ex: Lendor, o Errante">
        </div>

        <div class="duplo">
            <div class="linha">
                <div class="campo">
                    <label for="nivel">Nível</label>
                    <input type="number" id="nivel" min="0" max="60">
                </div>
            </div>
            <div class="linha">
                <div class="campo">
                    <label for="xp">XP</label>
                    <input type="number" id="xp">
                </div>
            </div>
        </div>

        <div class="duplo">
            <div class="campo">
                <label for="raca">Raça</label>
                <select id="raca"></select>
            </div>

            <div class="campo">
                <label for="classePersonagem">Classe</label>
                <select id="classePersonagem"></select>
            </div>
        </div>

        <div class="duplo">
            <div class="campo">
                <label for="origem">Origem</label>
                <input type="text" id="origem" placeholder="Ex: Eremita">
            </div>

            <div class="campo">
                <label for="divindade">Divindade</label>
                <input type="text" id="divindade" placeholder="Ex: São Nikolai">
            </div>
        </div>

        <div class="atributos">
            <div class="campo-atributo">
                <label for="for">FOR</label>
                <input type="number" id="for" min="-10" max="10">
            </div>
            <div class="campo-atributo">
                <label for="des">DES</label>
                <input type="number" id="des" min="-10" max="10">
            </div>
            <div class="campo-atributo">
                <label for="con">CON</label>
                <input type="number" id="con" min="-10" max="10">
            </div>
            <div class="campo-atributo">
                <label for="int">INT</label>
                <input type="number" id="int" min="-10" max="10">
            </div>
            <div class="campo-atributo">
                <label for="sen">SEN</label>
                <input type="number" id="sen" min="-10" max="10">
            </div>
            <div class="campo-atributo">
                <label for="car">CAR</label>
                <input type="number" id="car" min="-10" max="10">
            </div>
        </div>

        <div class="triplo">
            <div class="campo">
                <label for="pvAtual">PV Atual</label>
                <input type="number" id="pvAtual">
            </div>
            <div class="campo">
                <label for="pvMax">PV Máx</label>
                <input type="number" id="pvMax" readonly>
            </div>
            <div class="campo">
                <label for="pvTemp">PV Temp</label>
                <input type="number" id="pvTemp">
            </div>
        </div>

        <div class="triplo">
            <div class="campo">
                <label for="pmAtual">PM Atual</label>
                <input type="number" id="pmAtual">
            </div>
            <div class="campo">
                <label for="pmMax">PM Máx</label>
                <input type="number" id="pmMax" readonly>
            </div>
            <div class="campo">
                <label for="pmTemp">PM Temp</label>
                <input type="number" id="pmTemp">
            </div>
        </div>

        <div class="duplo">
            <div class="campo">
                <label for="pvExtra">PV Extra (racial, talentos, etc)</label>
                <input type="number" id="pvExtra" min="0" value="0">
            </div>

            <div class="campo">
                <label for="pmExtra">PM Extra (itens, talentos, etc)</label>
                <input type="number" id="pmExtra" min="0" value="0">
            </div>
        </div>

        <div class="triplo">
            <div class="campo">
                <label for="deslocamento">Deslocamento </label>
                <input type="text" id="deslocamento" min="0" max="60" placeholder="5 vk (7,5m)">
            </div>

            <div class="campo">
                <label for="tamanhoPersonagem">Tamanho</label>
                <select id="tamanhoPersonagem">
                    <option>Médio</option>
                    <option>Minúsculo</option>
                    <option>Pequeno</option>
                    <option>Grande</option>
                    <option>Colossal</option>
                </select>
            </div>

            <div class="campo">
                <label for="armadura">Armadura </label>
                <input type="text" id="armadura" placeholder="RD e Penalidade">
            </div>
        </div>

        <div class="duplo">
            <div class="linha-pericia">
                <div class="campo-pericia"><label>Defesa</label></div>
                <div class="campo-pericia4">
                    <select class="pericia-defesa">
                        <option value="Reflexos">Esquiva</option>
                        <option value="Fortitude">Vigor</option>
                        <option value="Vontade">Sanidade</option>
                    </select>
                </div>
                <div class="campo-pericia4"><input type="number" class="aparo" placeholder="Bônus de Aparo"></div>
                <div class="campo-pericia5"><input type="number" id="defesaFinal" readonly></div>
            </div>

            <div class="linha-pericia">
                <div class="campo-pericia"><label>Iniciativa</label></div>
                <div class="campo-pericia4">
                    <select class="pericia-iniciativa">
                        <option value="Percepção">Percepção</option>
                        <option value="Reflexos">Reflexos</option>
                        <option value="Intuição">Intuição</option>
                        <option value="Furtividade">Furtividade</option>
                        <option value="Atletismo">Atletismo</option>
                        <option value="Enganação">Enganação</option>
                        <option value="Intimidação">Intimidação</option>
                        <option value="Sobrevivência">Sobrevivência</option>
                        <option value="Acrobacia">Acrobacia</option>
                        <option value="Conh. C">Outro</option>
                    </select>
                </div>
                <div class="campo-pericia4"><input type="number" class="bonus-iniciativa" placeholder="Bônus de Iniciativa"></div>
                <div class="campo-pericia5"><input type="number" id="iniciativaFinal" readonly></div>
            </div>
        </div>

        <div class="campo">
            <label for="ataques">Ataques</label>
            <textarea id="ataques" rows="7">-> Espada Longa: d20+8+2 / 1d8+4+3</textarea>
        </div>

        <div>
            <div class="campo-atributo"><label for="pericias">Perícias</label></div>
            <div class="pericias" id="pericias-container"></div>
        </div>

        <div class="campo">
            <div class="campo-atributo"><label for="talentos">Talentos</label></div>
            <textarea id="talentos" rows="22"> -> Origem: 
 -> Raça: Idiomas, Visão, etc
 -> NV1: 
 -> NV2: 
 -> NV3: 
 -> NV4: 
 -> NV5: 
</textarea>
        </div>

        <div class="campo">
            <div class="campo-atributo"><label for="inventario">Inventário</label></div>
            <textarea id="inventario" rows="15"> -> Sigreis: 30§ </textarea>
        </div>

        <div class="campo">
            <div class="campo-atributo"><label for="magias">Magias</label></div>
            <textarea id="magias" rows="15"> -> 1° Círculo (Cargas: 6/6 )</textarea>

            <div class="linha-pericia">
                <div class="campo-pericia"><label>CD Conjuração</label></div>
                <div class="campo-pericia4"><input type="number" class="bonus-conjuracao" placeholder="Bônus na CD de Conjuração"></div>
                <div class="campo-pericia3"><input type="number" id="conjuracaoFinal" readonly></div>
            </div>
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
        /***********************
         * dados das perícias
         ************************/
        const pericias = [{
                nome: "Fortitude",
                atributo: "con"
            },
            {
                nome: "Percepção",
                atributo: "sen"
            },
            {
                nome: "Reflexos",
                atributo: "des"
            },
            {
                nome: "Luta",
                atributo: "for"
            },
            {
                nome: "Vontade",
                atributo: "car"
            },
            {
                nome: "Pontaria",
                atributo: "des"
            },
            {
                nome: "Acrobacia",
                atributo: "des"
            },
            {
                nome: "Arcanismo",
                atributo: "int"
            },
            {
                nome: "Adestramento",
                atributo: "car"
            },
            {
                nome: "Atletismo",
                atributo: "for"
            },
            {
                nome: "Atuação",
                atributo: "car"
            },
            {
                nome: "Cavalgar",
                atributo: "des"
            },
            {
                nome: "Conh.Alquimia",
                atributo: "int"
            },
            {
                nome: "Conh. Guerra",
                atributo: "int"
            },
            {
                nome: "Conh. Nobreza",
                atributo: "int"
            },
            {
                nome: "Conh. A",
                atributo: "int"
            },
            {
                nome: "Conh. B",
                atributo: "int"
            },
            {
                nome: "Conh. C",
                atributo: "int"
            },
            {
                nome: "Conh. D",
                atributo: "int"
            },
            {
                nome: "Conjuração",
                atributo: "int"
            },
            {
                nome: "Enganação",
                atributo: "car"
            },
            {
                nome: "Fabricação",
                atributo: "int"
            },
            {
                nome: "Furtividade",
                atributo: "des"
            },
            {
                nome: "Intimidação",
                atributo: "car"
            },
            {
                nome: "Intuição",
                atributo: "sen"
            },
            {
                nome: "Investigação",
                atributo: "int"
            },
            {
                nome: "Jogatina",
                atributo: "car"
            },
            {
                nome: "Ladinagem",
                atributo: "des"
            },
            {
                nome: "Medicina",
                atributo: "int"
            },
            {
                nome: "Natureza",
                atributo: "int"
            },
            {
                nome: "Ocultismo",
                atributo: "int"
            },
            {
                nome: "Persuasão",
                atributo: "car"
            },
            {
                nome: "Pilotagem",
                atributo: "des"
            },
            {
                nome: "Religião",
                atributo: "int"
            },
            {
                nome: "Sobrevivência",
                atributo: "sen"
            },
            {
                nome: "Sociedade",
                atributo: "int"
            }
        ];

        const atributos = [{
                value: "des",
                text: "DES"
            },
            {
                value: "for",
                text: "FOR"
            },
            {
                value: "con",
                text: "CON"
            },
            {
                value: "int",
                text: "INT"
            },
            {
                value: "sen",
                text: "SEN"
            },
            {
                value: "car",
                text: "CAR"
            }
        ];

        const treinamentos = [{
                value: "0",
                text: "Destreinado"
            },
            {
                value: "2",
                text: "Treinado"
            },
            {
                value: "4",
                text: "Especialista (ND7)"
            },
            {
                value: "6",
                text: "Mestre (ND13)"
            },
            {
                value: "8",
                text: "Lendário (ND18)"
            }
        ];

        function criarPericia(pericia, idx) {
            return `
        <div class="pericia" data-nome="${pericia.nome}">
          <div class="linha-pericia">
            <div class="campo-pericia"><label>${pericia.nome}</label></div>
            <div class="campo-pericia2">
              <select class="atributo-pericia">
                ${atributos.map(a => `<option value="${a.value}" ${a.value === pericia.atributo ? 'selected' : ''}>${a.text}</option>`).join('')}
              </select>
            </div>
            <div class="campo-pericia2">
              <select class="treinamento-pericia">
                ${treinamentos.map(t => `<option value="${t.value}">${t.text}</option>`).join('')}
              </select>
            </div>
            <div class="campo-pericia2">
              <input type="number" class="bonus-pericia" placeholder="Bônus">
            </div>
            <div class="campo-pericia3">
              <input type="number" class="valor-pericia" readonly>
            </div>
          </div>
        </div>
      `;
        }

        // renderiza perícias
        document.getElementById('pericias-container').innerHTML = pericias.map(criarPericia).join('');

        /***********************
         * lógica e persistência
         ************************/
        // popula raças e classes
        const racas = ["Humano", "Anão", "Elfo", "Forâneo", "Feral", "Gigante", "Goblin", "Golem", "Halfling", "Orc", "Troll"];
        const selectRaca = document.getElementById('raca');
        selectRaca.innerHTML = '<option value="">-- Selecione a Raça --</option>';
        racas.forEach(r => selectRaca.innerHTML += `<option>${r}</option>`);

        const classes = ["Bárbaro", "Bardo", "Bruxo", "Clérigo", "Combatente", "Druida", "Especialista", "Feiticeiro", "Inventor", "Investigador", "Ladino", "Lutador", "Mágico", "Mago", "Místico", "Oráculo", "Paladino", "Patrulheiro"];
        const selectClasse = document.getElementById('classePersonagem');
        selectClasse.innerHTML = '<option value="">-- Selecione a Classe --</option>';
        classes.forEach(c => selectClasse.innerHTML += `<option>${c}</option>`);

        // bases
        const BASES_PV = {
            'Bárbaro': 12,
            'Bruxo': 6,
            'Combatente': 10,
            'Lutador': 10,
            'Feiticeiro': 6,
            'Mago': 6,
            'Místico': 10,
            'Paladino': 10,
            'Patrulheiro': 10
        };
        const BASES_PM = {
            'Bardo': 4,
            'Bruxo': 5,
            'Druida': 4,
            'Feiticeiro': 5,
            'Mago': 5,
            'Clérigo': 4,
            'Oráculo': 4
        };

        function ajustarValorAtual(idElemento, valorMax) {
            const elemento = document.getElementById(idElemento);
            if (!elemento.value || parseInt(elemento.value) > valorMax) elemento.value = valorMax;
        }

        function calcularAtributos() {
            const constituicao = parseInt(document.getElementById('con').value) || 0;
            const nivel = parseInt(document.getElementById('nivel').value) || 1;
            const classe = document.getElementById('classePersonagem').value; // corrigido
            const pvExtra = parseInt(document.getElementById('pvExtra').value) || 0;
            const pmExtra = parseInt(document.getElementById('pmExtra').value) || 0;

            const basePV = BASES_PV[classe] || 8;
            const pvMax = (basePV + constituicao) * nivel + pvExtra;
            document.getElementById('pvMax').value = pvMax;

            const basePM = BASES_PM[classe] || 2;
            const pmMax = basePM * nivel + pmExtra;
            document.getElementById('pmMax').value = pmMax;

            ajustarValorAtual('pvAtual', pvMax);
            ajustarValorAtual('pmAtual', pmMax);
        }

        function atualizarPericias() {
            const nivel = parseInt(document.getElementById('nivel').value) || 0;
            const atributosVals = {
                for: parseInt(document.getElementById('for').value) || 0,
                des: parseInt(document.getElementById('des').value) || 0,
                con: parseInt(document.getElementById('con').value) || 0,
                int: parseInt(document.getElementById('int').value) || 0,
                sen: parseInt(document.getElementById('sen').value) || 0,
                car: parseInt(document.getElementById('car').value) || 0
            };

            document.querySelectorAll('.pericia').forEach(div => {
                const atributo = div.querySelector('.atributo-pericia').value;
                const treinamento = parseInt(div.querySelector('.treinamento-pericia').value) || 0;
                const bonusAdicional = parseInt(div.querySelector('.bonus-pericia').value) || 0;
                const baseNivel = (treinamento === 0) ? Math.floor(nivel / 2) : Math.floor(nivel);
                const valor = baseNivel + (atributosVals[atributo] || 0) + treinamento + bonusAdicional;
                const out = div.querySelector('.valor-pericia');
                if (out) out.value = valor;
            });
        }

        // eventos
        const idsParaCalculo = ['nivel', 'for', 'des', 'con', 'int', 'sen', 'car'];
        idsParaCalculo.forEach(id => {
            const el = document.getElementById(id);
            if (el) el.addEventListener('input', () => {
                atualizarPericias();
                calcularDefesa();
                calcularIniciativa();
                calcularCDConjuracao();
            });
        });

        // eventos mais específicos (delegação)
        document.addEventListener('change', e => {
            const t = e.target;
            if (!t) return;
            if (t.classList && (t.classList.contains('atributo-pericia') || t.classList.contains('pericia-iniciativa') || t.classList.contains('pericia-defesa') || t.classList.contains('treinamento-pericia') || t.classList.contains('bonus-pericia'))) {
                atualizarPericias();
                calcularDefesa();
                calcularIniciativa();
                calcularCDConjuracao();
            }
        });

        document.querySelectorAll('.bonus-pericia').forEach(inp => inp.addEventListener('input', atualizarPericias));
        if (document.querySelector('.bonus-iniciativa')) document.querySelector('.bonus-iniciativa').addEventListener('input', calcularIniciativa);
        if (document.querySelector('.bonus-conjuracao')) document.querySelector('.bonus-conjuracao').addEventListener('input', calcularCDConjuracao);
        if (document.querySelector('.aparo')) document.querySelector('.aparo').addEventListener('input', calcularDefesa);
        if (document.querySelector('.pericia-defesa')) document.querySelector('.pericia-defesa').addEventListener('change', calcularDefesa);
        if (document.querySelector('.pericia-iniciativa')) document.querySelector('.pericia-iniciativa').addEventListener('change', calcularIniciativa);

        function calcularDefesa() {
            const base = 10;
            const aparo = parseInt(document.querySelector('.aparo').value) || 0;
            const defesaTipo = document.querySelector('.pericia-defesa').value;
            const periciasMap = {};
            document.querySelectorAll('.pericia').forEach(div => {
                const nome = div.querySelector("label").innerText.trim();
                const valor = parseInt(div.querySelector(".valor-pericia").value) || 0;
                periciasMap[nome] = valor;
            });
            const valorPericia = periciasMap[defesaTipo] || 0;
            document.getElementById("defesaFinal").value = base + aparo + valorPericia;
        }

        function calcularIniciativa() {
            const bonusIniciativa = parseInt(document.querySelector('.bonus-iniciativa').value) || 0;
            const periciaIniciativa = document.querySelector('.pericia-iniciativa').value;
            const periciasMap = {};
            document.querySelectorAll('.pericia').forEach(div => {
                const nome = div.querySelector("label").innerText.trim();
                const valor = parseInt(div.querySelector(".valor-pericia").value) || 0;
                periciasMap[nome] = valor;
            });
            const valorPericia = periciasMap[periciaIniciativa] || 0;
            document.getElementById("iniciativaFinal").value = bonusIniciativa + valorPericia;
        }

        function calcularCDConjuracao() {
            const base = 10;
            const bonusConjuracao = parseInt(document.querySelector('.bonus-conjuracao').value) || 0;
            const periciasMap = {};
            document.querySelectorAll('.pericia').forEach(div => {
                const nome = div.querySelector("label").innerText.trim();
                const valor = parseInt(div.querySelector(".valor-pericia").value) || 0;
                periciasMap[nome] = valor;
            });
            let valorPericia = 0;
            for (const key in periciasMap) {
                if (key.toLowerCase() === "conjuração".toLowerCase()) {
                    valorPericia = periciasMap[key];
                    break;
                }
            }
            document.getElementById("conjuracaoFinal").value = base + valorPericia + bonusConjuracao;
        }

        // salvar local (opcional)
        function salvarFicha() {
            const campos = document.querySelectorAll('input, select, textarea');
            campos.forEach(el => {
                if (el.id) localStorage.setItem('ficha-' + el.id, el.value);
            });

            // salva perícias
            const periciasData = [];
            document.querySelectorAll('.pericia').forEach(div => {
                const nome = div.dataset.nome;
                const atributo = div.querySelector('.atributo-pericia').value;
                const treinamento = div.querySelector('.treinamento-pericia').value;
                const bonus = div.querySelector('.bonus-pericia').value;
                const valor = div.querySelector('.valor-pericia').value;
                periciasData.push({
                    nome,
                    atributo,
                    treinamento,
                    bonus,
                    valor
                });
            });
            localStorage.setItem('ficha-pericias', JSON.stringify(periciasData));
            alert("Ficha salva nas memórias do grimório!");
        }

        // exportar (gera JSON com perícias completas)
        function baixarFicha() {
            const campos = document.querySelectorAll('input, select, textarea');
            const ficha = {};
            campos.forEach(el => {
                if (el.id) ficha[el.id] = (el.type === 'checkbox') ? el.checked : el.value;
            });

            ficha.pericias = [];
            document.querySelectorAll('.pericia').forEach(div => {
                const nome = div.dataset.nome;
                const atributo = div.querySelector('.atributo-pericia').value;
                const treinamento = div.querySelector('.treinamento-pericia').value;
                const bonus = div.querySelector('.bonus-pericia').value;
                const valor = div.querySelector('.valor-pericia').value;
                ficha.pericias.push({
                    nome,
                    atributo,
                    treinamento,
                    bonus,
                    valor
                });
            });

            const blob = new Blob([JSON.stringify(ficha, null, 2)], {
                type: 'application/json'
            });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');

            let nome = document.getElementById('nome').value.trim();
            if (!nome) nome = 'personagem';
            nome = nome.replace(/[\/\\:\*\?"<>\|]/g, '');

            a.href = url;
            a.download = nome + '_ficha_auramana_pf2e.json';
            a.click();
            URL.revokeObjectURL(url);
        }

        // importar arquivo JSON (preenche campos e perícias)
        function carregarFicha() {
            const input = document.getElementById('uploadFicha');
            const file = input.files[0];
            if (!file) return;

            const reader = new FileReader();
            reader.onload = function(e) {
                let data;
                try {
                    data = JSON.parse(e.target.result);
                } catch (err) {
                    alert('Arquivo JSON inválido.');
                    return;
                }

                // campos simples
                Object.keys(data).forEach(key => {
                    if (key === 'pericias') return;
                    const el = document.getElementById(key);
                    if (el) {
                        if (el.type === 'checkbox') el.checked = data[key];
                        else el.value = data[key];
                        // atualiza localStorage também
                        if (el.id) localStorage.setItem('ficha-' + el.id, el.value);
                    }
                });

                // perícias
                if (Array.isArray(data.pericias)) {
                    data.pericias.forEach(pd => {
                        const div = Array.from(document.querySelectorAll('.pericia')).find(d => d.dataset.nome === pd.nome);
                        if (!div) return;
                        const attrSel = div.querySelector('.atributo-pericia');
                        if (attrSel && pd.atributo) attrSel.value = pd.atributo;

                        const trainSel = div.querySelector('.treinamento-pericia');
                        if (trainSel && (pd.treinamento !== undefined && pd.treinamento !== null)) {
                            // tenta casar por value
                            const hasValue = Array.from(trainSel.options).some(o => o.value == pd.treinamento);
                            if (hasValue) trainSel.value = String(pd.treinamento);
                            else {
                                // tenta casar por texto
                                const opt = Array.from(trainSel.options).find(o => o.text == pd.treinamento);
                                if (opt) trainSel.value = opt.value;
                            }
                        }

                        const bonus = div.querySelector('.bonus-pericia');
                        if (bonus && pd.bonus !== undefined) bonus.value = pd.bonus;

                        const valor = div.querySelector('.valor-pericia');
                        if (valor && pd.valor !== undefined) valor.value = pd.valor;
                    });

                    // salvar perícias no localStorage
                    localStorage.setItem('ficha-pericias', JSON.stringify(data.pericias));
                }

                alert('Ficha carregada com sucesso!');
                atualizarPericias();
                calcularDefesa();
                calcularIniciativa();
                calcularCDConjuracao();
            };
            reader.readAsText(file);
        }

        function limparFicha() {
            if (!confirm("Tem certeza que deseja apagar todos os dados da ficha?")) return;
            const campos = document.querySelectorAll('input, select, textarea');
            campos.forEach(el => {
                localStorage.removeItem('ficha-' + el.id);
                if (el.type === 'checkbox') el.checked = false;
                else if (el.tagName === 'SELECT') el.selectedIndex = 0;
                else el.value = '';
            });
            localStorage.removeItem('ficha-pericias');
            alert("Todos os dados foram apagados da ficha.");
        }

        // restaura do localStorage ao abrir
        window.addEventListener('DOMContentLoaded', () => {
            // campos
            const campos = document.querySelectorAll('input, select, textarea');
            campos.forEach(el => {
                if (!el.id) return;
                const val = localStorage.getItem('ficha-' + el.id);
                if (val !== null) el.value = val;
            });

            // perícias
            const periciasSalvas = JSON.parse(localStorage.getItem('ficha-pericias') || '[]');
            periciasSalvas.forEach(pd => {
                const div = Array.from(document.querySelectorAll('.pericia')).find(d => d.dataset.nome === pd.nome);
                if (!div) return;
                if (pd.atributo) div.querySelector('.atributo-pericia').value = pd.atributo;
                const trainSel = div.querySelector('.treinamento-pericia');
                if (trainSel && pd.treinamento !== undefined) {
                    const hasValue = Array.from(trainSel.options).some(o => o.value == pd.treinamento);
                    if (hasValue) trainSel.value = String(pd.treinamento);
                }
                if (pd.bonus !== undefined) div.querySelector('.bonus-pericia').value = pd.bonus;
                if (pd.valor !== undefined) div.querySelector('.valor-pericia').value = pd.valor;
            });

            atualizarPericias();
            calcularDefesa();
            calcularIniciativa();
            calcularCDConjuracao();
            calcularAtributos();
        });

        // para garantir recalculo caso window.onload seja usado
        window.onload = () => {
            // garante que valores salvos sejam aplicados (zeros também)
            const campos = document.querySelectorAll('input, select, textarea');
            campos.forEach(el => {
                if (!el.id) return;
                const val = localStorage.getItem('ficha-' + el.id);
                if (val !== null) el.value = val;
            });
            atualizarPericias();
            calcularDefesa();
            calcularIniciativa();
            calcularCDConjuracao();
        };
    </script>
</body>

</html>