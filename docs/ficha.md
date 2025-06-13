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
      grid-template-columns: repeat(2, 1fr);
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
        <option>Feral</option>
        <option>Extraplanar</option>

      </select>
    </div>

    <div class="campo">
      <label for="classe">Classe</label>
      <select id="classe">
        <option value="">-- Selecione a Classe --</option>
        <option>Arcanista</option>
        <option>Batedor</option>
        <option>Guerreiro</option>
        <option>Elementalista</option>
        <option>Inspirador</option>
        <option>Inventor</option>
        <option>Sacerdote</option>
      </select>
    </div>

    <div class="campo">
      <label for="arquetipo">Arquétipo</label>
      <select id="arquetipo">
        <option value="">-- Selecione o Arquétipo --</option>
        <optgroup label="Arcanista">
          <option>Bruxo</option><option>Feiticeiro</option><option>Mago</option><option>Necromante</option>
        </optgroup>
        <optgroup label="Batedor">
          <option>Bucaneiro</option><option>Caçador</option><option>Duelista</option><option>Investigador</option><option>Ladino</option><option>Ventanista</option>
        </optgroup>
        <optgroup label="Elementalista">
          <option>Druida</option><option>Místico</option><option>Treinador</option>
        </optgroup>
        <optgroup label="Guerreiro">
          <option>Bárbaro</option><option>Cavaleiro</option><option>Lutador</option><option>Samurai</option><option>Soldado</option>
        </optgroup>
        <optgroup label="Inspirador">
          <option>Bardo</option><option>Nobre</option><option>Oráculo</option>
        </optgroup>
        <optgroup label="Inventor">
          <option>Alquimista</option><option>Artilheiro</option><option>Ferreiro</option>
        </optgroup>
        <optgroup label="Sacerdote">
          <option>Clérigo</option><option>Frade</option><option>Paladino</option><option>Santo</option>
        </optgroup>
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

    <div class="linha">
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
        <option>Minúsculo</option>
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
        
    <h2>Perícias</h2>
    
    <div class="pericias">
        
      <div class="pericia">
        <label>Acrobacia</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Adestramento</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Atlestimo</label>
        <select class="atributo-pericia">
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Atuação</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

      <div class="pericia">
        <label>Cavalgar</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Conhecimento</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Cura</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
            
       <div class="pericia">
        <label>Diplomacia</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Enganação</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Fortitude</label>
        <select class="atributo-pericia">
          <option value="con">CON</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Furtividade</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Guerra</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Iniciativa</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Intimidação</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Intuição</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Investigação</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
            
       <div class="pericia">
        <label>Jogatina</label>
        <select class="atributo-pericia">
          <option value="car">CAR</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Ladinagem</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Luta</label>
        <select class="atributo-pericia">
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Misticismo</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>

       <div class="pericia">
        <label>Nobreza</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Ofício Alquimia</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Ofício Artilheiro</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Ofício Engenhoqueiro</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Ofício Ferreiro</label>
        <select class="atributo-pericia">
          <option value="int">INT</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>            
      
      <div class="pericia">
        <label>Percepção</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Pilotagem</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
      <div class="pericia">
        <label>Pontaria</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div> 
      
      <div class="pericia">
        <label>Reflexos</label>
        <select class="atributo-pericia">
          <option value="des">DES</option>
          <option value="for">FOR</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="sab">SAB</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Religião</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
            
       <div class="pericia">
        <label>Sobrevivência</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
       <div class="pericia">
        <label>Vontade</label>
        <select class="atributo-pericia">
          <option value="sab">SAB</option>
          <option value="for">FOR</option>
          <option value="des">DES</option>
          <option value="con">CON</option>
          <option value="int">INT</option>
          <option value="car">CAR</option>
        </select>
        <select class="treinamento-pericia">
          <option value="0">Destreinado</option>
          <option value="2">Iniciante</option>
          <option value="4">Veterano (ND7)</option>
          <option value="6">Mestre (ND13)</option>
        </select>
        <input type="number" class="bonus-pericia" placeholder="Bônus de Perícia">
        <input type="number" class="valor-pericia" readonly>
      </div>
      
    </div>
    </div>
 </div>


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
</textarea>
</div>

<div class="campo">
  <label for="magias">Magias</label>
  <textarea id="poderes" rows="22">
 -> 1° Círculo:
 -
 -> 2° Círculo:
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
  const nome = document.getElementById('nome');
  a.download = nome + 'ficha_t20.json';
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

