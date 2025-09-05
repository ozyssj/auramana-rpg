<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <title>Ficha de Personagem - Auramana Pathfinder</title>
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
            gap: 15px;
            width: 100%;
            overflow: hidden;
        }

        .pericia {
            min-width: 0;
            break-inside: avoid;
            page-break-inside: avoid;
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
            <select id="raca"></select>
        </div>

        <div class="campo">
            <label for="classe">Classe</label>
            <select id="classe"></select>
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
                <label for="sen">SEN</label>
                <input type="number" id="sen" min="-10" max="10">
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
                <input type="number" id="pvMax" readonly>
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
                <input type="number" id="pmMax" readonly>
            </div>
            <div class="campo">
                <label for="pmTemp">PM Temp</label>
                <input type="number" id="pmTemp">
            </div>
        </div>

        <div class="linha">
            <div class="campo">
                <label for="pvExtra">PV Extra (racial, poderes, etc)</label>
                <input type="number" id="pvExtra" min="0" value="0">
            </div>

            <div class="campo">
                <label for="pmExtra">PM Extra (conjuração, poderes, etc)</label>
                <input type="number" id="pmExtra" min="0" value="0">
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

 
                <div class="linha">
                    <div class="campo">
                        <label>Defesa</label>
                        <select class="pericia-defesa">
                                  <option value="Reflexos">Reflexos</option>
                                  <option value="Fortitude">Fortitude</option>
                                  <option value="Vontade">Vontade</option>
                        </select>
                        <input type="number" class="aparo" placeholder="Bônus de Aparo">
                        <input type="number" id="defesaFinal" readonly>
                    </div>
                </div>



                <div class="linha">
                    <div class="campo">
                        <label>Iniciativa</label>
                        <select class="pericia-iniciativa">
                                  <option value="Reflexos">Reflexos</option>
                                  <option value="Fortitude">Fortitude</option>
                                  <option value="Vontade">Vontade</option>
                        </select>
                        <input type="number" class="bonus-iniciativa" placeholder="Bônus de Iniciativa">
                       <input type="number" id="iniciativaFinal" readonly>            
                    </div>
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
                        { nome: "Acrobacia", atributo: "des" },
                        { nome: "Arcanismo", atributo: "int" },
                        { nome: "Adestramento", atributo: "car" },
                        { nome: "Atletismo", atributo: "for" },
                        { nome: "Atuação", atributo: "car" },
                        { nome: "Cavalgar", atributo: "des" },
                        { nome: "Conhecimento em Alquimia", atributo: "int" },
                        { nome: "Conhecimento em Guerra", atributo: "int" },
                        { nome: "Conhecimento em Nobreza", atributo: "int" },
                        { nome: "Conjuração", atributo: "int" },
                        { nome: "Enganação", atributo: "car" },
                        { nome: "Fortitude", atributo: "con" },
                        { nome: "Furtividade", atributo: "des" },
                        { nome: "Intimidação", atributo: "car" },
                        { nome: "Intuição", atributo: "sen" },
                        { nome: "Investigação", atributo: "int" },
                        { nome: "Ladinagem", atributo: "des" },
                        { nome: "Luta", atributo: "for" },
                        { nome: "Medicina", atributo: "int" },
                        { nome: "Natureza", atributo: "int" },
                        { nome: "Ocultismo", atributo: "int" },
                        { nome: "Percepção", atributo: "sen" },
                        { nome: "Persuasão", atributo: "car" },
                        { nome: "Pilotagem", atributo: "des" },
                        { nome: "Pontaria", atributo: "des" },
                        { nome: "Reflexos", atributo: "des" },
                        { nome: "Religião", atributo: "int" },
                        { nome: "Sobrevivência", atributo: "sen" },
                        { nome: "Sociedade", atributo: "int" },
                        { nome: "Vontade", atributo: "car" }
                    ];

                    // Opções de atributos
                    const atributos = [
                        { value: "des", text: "DES" },
                        { value: "for", text: "FOR" },
                        { value: "con", text: "CON" },
                        { value: "int", text: "INT" },
                        { value: "sen", text: "SEN" },
                        { value: "car", text: "CAR" }
                    ];

                    // Opções de treinamento
                    const treinamentos = [
                        { value: "0", text: "Destreinado" },
                        { value: "2", text: "Treinado" },
                        { value: "4", text: "Especialista (ND7)" },
                        { value: "6", text: "Mestre (ND13)" },
                        { value: "8", text: "Lendário (ND18)" }
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
                    <button onclick="document.getElementById('uploadFicha').click()">Importar
                        Ficha</button>
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
                        sen: parseInt(document.getElementById('sen').value) || 0,
                        car: parseInt(document.getElementById('car').value) || 0
                    };

                    document.querySelectorAll('.pericia').forEach(div => {
                        const atributo = div.querySelector('.atributo-pericia').value;
                        const treinamento = parseInt(div.querySelector('.treinamento-pericia').value);
                        const bonusAdicional = parseInt(div.querySelector('.bonus-pericia').value) || 0;
                        const baseNivel = (treinamento === 0) ? Math.floor(nivel / 2) : Math.floor(nivel);
                        const valor = baseNivel + atributos[atributo] + treinamento + bonusAdicional;
                        div.querySelector('.valor-pericia').value = valor;
                    });
                }

                ['nivel', 'for', 'des', 'con', 'int', 'sen', 'car'].forEach(id => {
                    document.getElementById(id).addEventListener('input', atualizarPericias);
                });

                document.addEventListener('change', e => {
                    if (e.target.classList.contains('atributo-pericia') || e.target.classList.contains('pericia-iniciativa') || e.target.classList.contains('pericia-defesa') || e.target.classList.contains('treinamento-pericia') || e.target.classList.contains('bonus-pericia'
                    
                    )) {
                        atualizarPericias();
                        calcularDefesa();
                        calcularIniciativa();
                    }
                });
                
                document.querySelectorAll('.bonus-pericia').forEach(input => {
                    input.addEventListener('input', atualizarPericias);
                });
                document.querySelector('.bonus-iniciativa').addEventListener('input', calcularIniciativa);
                document.querySelector('.aparo').addEventListener('input', calcularDefesa);
                document.querySelector('.pericia-defesa').addEventListener('change', calcularDefesa);
                document.querySelector('.pericia-iniciativa').addEventListener('change', calcularDefesa);

                function calcularDefesa() {
                    const base = 10;

                    // pega bônus extra de defesa (campo manual)
                    const aparo = parseInt(document.querySelector('.aparo').value) || 0;

                    // pega qual perícia foi escolhida
                    const defesaTipo = document.querySelector('.pericia-defesa').value;

                    // mapeia todas as perícias calculadas
                    const periciasMap = {};
                    document.querySelectorAll('.pericia').forEach(div => {
                        const nome = div.querySelector("label").innerText.trim();
                        const valor = parseInt(div.querySelector(".valor-pericia").value) || 0;
                        periciasMap[nome] = valor;
                    });

                    // pega só a escolhida
                    const valorPericia = periciasMap[defesaTipo] || 0;

                    // soma tudo
                    const defesaFinal = base + aparo + valorPericia;
                    document.getElementById("defesaFinal").value = defesaFinal;
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

                    const iniciativaFinal = bonusIniciativa + valorPericia;
                    document.getElementById("iniciativaFinal").value = iniciativaFinal;
                }


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
                
                

                const racas = [
                    "Humano", "Anão", "Elfo", "Forâneo", "Feral", "Gigante", "Goblin", "Halfling", "Orc", "Troll"
                ];

                const selectRaca = document.getElementById('raca');

                selectRaca.innerHTML = '<option value="">-- Selecione a Raça --</option>';

                racas.forEach(raca => {
                    selectRaca.innerHTML += `<option>${raca}</option>`;
                });


                const classes = [
                    "Bárbaro", "Bardo", "Bruxo", "Clérigo", "Combatente", "Druida", "Feiticeiro", "Inventor", 
                    "Investigador", "Ladino", "Mago", "Místico", "Oráculo", "Paladino", "Patrulheiro"
                ];

                const selectClasse = document.getElementById('classe');

                selectClasse.innerHTML = '<option value="">-- Selecione a Classe --</option>';

                classes.forEach(classe => {
                    selectClasse.innerHTML += `<option>${classe}</option>`;
                });

                
                // Constantes com os valores base por classe
                const BASES_PV = {
                    'Bárbaro': 12,
                    'Bruxo': 6,
                    'Combatente': 10,
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

                // Função unificada para cálculos
                function calcularAtributos() {
                    const constituicao = parseInt(document.getElementById('con').value) || 0;
                    const nivel = parseInt(document.getElementById('nivel').value) || 1;
                    const classe = document.getElementById('classe').value;
                    const pvExtra = parseInt(document.getElementById('pvExtra').value) || 0;
                    const pmExtra = parseInt(document.getElementById('pmExtra').value) || 0;

                    // Cálculo de PV
                    const basePV = BASES_PV[classe] || 8;
                    const pvMax = (basePV + constituicao) * nivel + pvExtra;
                    document.getElementById('pvMax').value = pvMax;

                    // Cálculo de PM
                    const basePM = BASES_PM[classe] || 2;
                    const pmMax = basePM * nivel + pmExtra;
                    document.getElementById('pmMax').value = pmMax;

                    // Ajustar valores atuais
                    ajustarValorAtual('pvAtual', pvMax);
                    ajustarValorAtual('pmAtual', pmMax);
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
                    ['con', 'nivel', 'classe', 'pvExtra', 'pmExtra'].forEach(id => {
                        document.getElementById(id).addEventListener('input', calcularAtributos);
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
                    // Carregar valores salvos
                    if (localStorage.getItem('ficha-pvExtra')) {
                        document.getElementById('pvExtra').value = localStorage.getItem('ficha-pvExtra');
                    }
                    if (localStorage.getItem('ficha-pmExtra')) {
                        document.getElementById('pmExtra').value = localStorage.getItem('ficha-pmExtra');
                    }

                    // Configurar eventos e calcular valores iniciais
                    configurarEventos();
                    calcularAtributos();
                });

                window.onload = () => {
                    const campos = document.querySelectorAll('input, select, textarea');
                    campos.forEach(el => {
                        const val = localStorage.getItem('ficha-' + el.id);
                        if (val) el.value = val;
                    });
                    atualizarPericias();
                    calcularDefesa();
                    calcularIniciativa();
                };

            </script>
</body>

</html>