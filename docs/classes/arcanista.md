<!-- docs/classes/arcanista.md -->
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
    font-family: 'MedievalSharp', cursive;
    background-color: var(--cor-fundo);
    color: var(--cor-texto);
    line-height: 1.6;
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
  }

  .classe-header {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    border-bottom: 2px solid var(--cor-primaria);
    padding-bottom: 15px;
  }

  .classe-icon {
    width: 60px;
    height: 60px;
    margin-right: 20px;
    object-fit: contain;
  }

  .classe-info {
    background-color: rgba(187, 168, 140, 0.1);
    border-left: 4px solid var(--cor-primaria);
    border-radius: 0 5px 5px 0;
    padding: 15px;
    margin: 20px 0;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin: 20px 0;
    background-color: rgba(187, 168, 140, 0.05);
  }

  th, td {
    border: 1px solid var(--cor-destaque);
    padding: 8px 12px;
    text-align: left;
  }

  th {
    background-color: rgba(91, 70, 54, 0.2);
  }

  tr:nth-child(even) {
    background-color: rgba(187, 168, 140, 0.1);
  }

  h1, h2, h3 {
    color: var(--cor-primaria);
    text-shadow: 1px 1px var(--cor-destaque);
    border-bottom: 2px solid var(--cor-primaria);
    padding-bottom: 5px;
  }

  .habilidade {
    margin-bottom: 15px;
    padding-left: 10px;
    border-left: 3px solid var(--cor-destaque);
  }
</style>

<div class="classe-header">
  <img src="../../img/classes/arcanista.png" alt="Arcanista" class="classe-icon">
  <h1>Arcanista</h1>
</div>

<p><em>Mestres da magia erudita que dominam os segredos arcanos através de estudo e disciplina.</em></p>

<div class="classe-info">
  <h2>Características de Classe</h2>
  
  <h3>Pontos de Vida</h3>
  <p>3 PV (+ Constituição) por nível.</p>
  
  <h3>Pontos de Mana</h3>
  <p>6 PM por nível.</p>
  
  <h3>Perícias</h3>
  <p><strong>Treinadas:</strong> Misticismo (Int) e Vontade (Sab)</p>
  <p><strong>Escolha mais 4 entre:</strong> Conhecimento (Int), Diplomacia (Car), Enganação (Car), Guerra (Int), Iniciativa (Des), Intimidação (Car), Intuição (Sab), Investigação (Int), Nobreza (Int), Ofício (Int) e Percepção (Sab)</p>
  
  <h3>Proficiências</h3>
  <p>Nenhuma.</p>
</div>

<h2>Habilidades de Classe</h2>

<div class="habilidade">
  <h3>Magias</h3>
  <p>Você pode lançar magias arcanas de 1º círculo. A cada quatro níveis, pode lançar magias de um círculo maior (2º círculo no 5º nível, 3º círculo no 9º nível e assim por diante).</p>
  <p>Você começa com três magias de 1º círculo. A cada nível, aprende uma magia de qualquer círculo que possa lançar.</p>
  <p>Seu atributo-chave para lançar magias é definido pelo seu Arquétipo Arcano e você soma o bônus do atributo-chave no seu total de PM.</p>
</div>

<div class="habilidade">
  <h3>Raio Arcano</h3>
  <p>Escolha um tipo de dano entre fogo, ácido, relâmpago, frio, mental e essência. Uma vez feita a escolha, ela não pode ser alterada.</p>
  <p>Você pode gastar uma ação padrão para causar 1d8 pontos do dano escolhido num alvo em alcance curto. Esse dano aumenta em +1d8 para cada círculo de magia acima do 1º que você puder lançar.</p>
  <p>O alvo pode fazer um teste de Reflexos (CD atributo-chave) para reduzir o dano à metade. O Raio Arcano conta como uma magia para efeitos de habilidades e itens que beneficiem suas magias.</p>
  <p>Por fim, assim como magias com alvo único, você pode substituir o teste resistência do seu raio por um teste de ataque utilizando Misticismo (crítico x2).</p>
</div>

<!-- Continue com as outras habilidades seguindo o mesmo padrão -->

<h2>Tabela de Progressão</h2>

<table>
  <thead>
    <tr>
      <th>Nível</th>
      <th>Habilidades</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Magias (1º Círculo), Raio Arcano (1d8), Arquétipo Arcano</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Poder de Arcanista</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Arquétipo Arcano</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Aumento de Atributo</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Magias (2º Círculo), Raio Arcano (2d8), Fortalecimento Arcano</td>
    </tr>
    <!-- Continue com todas as linhas da tabela -->
    <tr>
      <td>20</td>
      <td>Alta Arcana, Poder de Arcanista</td>
    </tr>
  </tbody>
</table>

<h3>Arquétipos Arcanos (a serem detalhados)</h3>
<ul>
  <li><strong>Bruxo:</strong> Pactos com entidades misteriosas</li>
  <li><strong>Feiticeiro:</strong> Magia inata e metamágica</li>
  <li><strong>Mago:</strong> Conhecimento arcano e especialização</li>
</ul>



