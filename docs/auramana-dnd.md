<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Contos de Fantasia</title>
  <style>
    @import url('https://fonts.googleapis.com/css?family=Libre+Baskerville&display=swap');

    body {
      background: #f7ebcb; 
      font-family: 'Libre Baskerville', serif;
      font-size: 16px;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      margin: 20px;
      color: #3a2b17;
    }

    h1, h2, h3, h4, h5, h6 {
      color: #7a2b17; 
      text-transform: uppercase;
      line-height: 1.1;
      margin: 24px 0 12px 0;
    }

    h1::first-letter,
    h2::first-letter,
    h3::first-letter,
    h4::first-letter,
    h5::first-letter,
    h6::first-letter {
      font-size: 150%;
    }

    h1 {
      font-size: 24px;
      border-bottom: 2px solid tan; 
      padding-bottom: 6px;
      max-width: max-content;
    }

    h2 {
      border-bottom: 2px solid tan; 
      padding-bottom: 4px;
      max-width: max-content;
    }

    p {
      line-height: 1.4;
      margin: 0;
    }

    p + p {
      text-indent: 24px;
      margin-top: 0 !important;
    }

    .box {
      background-color: white;
      padding: 16px;
      border-left: 2px solid black;
      border-right: 2px solid black;
      overflow: hidden;
      margin: 16px 0;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
      border-radius: 4px;
    }
    
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1rem;
      margin-bottom: 1rem;
      background-color: #f7ebcb;
    }

    th, td {
      border: 1px solid #e0e5c1;
      padding: 8px 12px;
      text-align: left;
      vertical-align: top;
    }

    th {
      background-color: #e0e5c1;
      color: #3b170f;
    }

    td {
      background-color: #e0e5c1;
    }

    td2 {
      background-color: #f7ebcb;
    }
    
    
    a {
      color: #fffff;
      text-decoration: underline;
    }

    a:hover {
      color: #a63232;
    }    
    
  </style>
</head>



<body>

  <div class="wide">

    <h1>Auramana Versão D&D 2024</h1>

    <h2>Criação de Personagem</h2>

    <h3>Materiais Permitidos</h3>
    <table>
      <thead>
        <tr><th>Livro</th><th>Itens Permitidos</th></tr>
      </thead>
      <tbody>
        <tr><td>Livro do Jogador (2024)</td><td>Integral</td></tr>
        <tr><td>Livro dos Monstros</td><td>Integral</td></tr>
        <tr><td>Modern Handbook 5E</td><td>Integral (one-shots e campanhas modernas)</td></tr>
        <tr><td>Livro do Mestre</td><td>Clérigo (Morte), Paladino (Quebrador de Juramento)</td></tr>
        <tr><td>Livro do Jogador (2014)</td><td>Clérigo (Conhecimento, Morte, Natureza, Tempestade), Mago (Convocador, Encantador, Necromante, Transmutador)</td></tr>
        <tr><td>Guia do Aventureiro da Costa da Espada</td><td>Magias, Bárbaro (Besta), Bruxo (Imortal), Clérigo (Arcana), Guerreiro (Porta-Estandarte), Paladino (Coroa)</td></tr>
        <tr><td>Tesouro dos Dragões de Fizban</td><td>Magias, Guardião (Drakewarden), Monge (Dragão Ascendido)</td></tr>
        <tr><td>Caldeirão da Tasha Para Tudo</td><td>Magias, Artífice (Alquimista, Armeiro, Artilheiro, Ferreiro de Batalha), Bardo (Criação, Eloquência), Bárbaro (Magia Selvagem), Bruxo (Gênio, Insondável), Clérigo (Forja, Ordem, Paz), Druida (Esporos, Fogo Selvagem), Guardião (Guardião do Enxame), Ladino (Inquisitivo), Mago (Ordem dos Escribas), Monge (Projeção Astral)</td></tr>
        <tr><td>Presentes de Bigby: Glória dos Gigantes</td><td>Origens, Bárbaro (Gigante)</td></tr>
        <tr><td>Dragonlance: Sombra da Rainha Dragão</td><td>Feiticeiro (Feitiçaria Lunar)</td></tr>
        <tr><td>Guia Para Tudo de Xanathar</td><td>Magias, Bárbaro (Guardião Ancestral), Bardo (Espadas, Sussuros), Bruxo (Má-Lâmina), Druida (Pastoreio, Sonhos), Feiticeiro (Alma Divina, Feitiçaria da Tormenta, Magia Sombria), Guardião (Andarilho do Horizonte, Matador de Monstros), Guerreiro (Arqueiro Arcano, Cavaleiro, Samurai), Ladino (Batedor, Bucaneiro, Malfeitor), Mago (Magia de Guerra), Monge (Kensei, Mestre Bêbado), Paladino (Conquista, Redenção)</td></tr>
      </tbody>
    </table>

    <h3>Atributos</h3>
    <p>Utilize uma das seguintes combinações de valores de atributo:</p>
    <table>
      <tbody>
        <tr><td>15, 14, 13, 11, 10 e 9</td></tr>
        <tr><td>15, 15, 13, 10, 10 e 8</td></tr>
        <tr><td>15, 14, 13, 10, 10 e 10</td></tr>
      </tbody>
    </table>
    <p>
      Você pode utilizar a calculadora do 
      <a href="https://chicken-dinner.com/5e/5e-point-buy.html" target="_blank">Chicken Dinner</a>, 
      porém sem selecionar a raça.
    </p>
    <p>
      Alternativamente, utilize o método de rolagem: role 4d6 e some os três maiores resultados. Faça isso seis vezes.<br>
      Em seguida, aplique os aumentos de atributos da Origem.
    </p>

    <h3>Raças e Classes Permitidas</h3>
    <table>
      <thead>
        <tr><th>Raça</th><th>Classes</th></tr>
      </thead>
      <tbody>
        <tr><td>Humano</td><td>Qualquer</td></tr>
        <tr><td>Lobisomem</td><td>Bárbaro (qualquer), Druida (Lua, Pastoreio, Terra), Guardião (Caçador, Matador de Monstros, Senhor das Feras, Vigilante das Sombras)</td></tr>
        <tr><td>Vampiro</td><td>Qualquer</td></tr>
        <tr><td>Feérico</td><td>Qualquer</td></tr>
        <tr><td>Monstro</td><td>Qualquer</td></tr>
        <tr><td>Múmia</td><td>Clérigo (qualquer), Guerreiro (qualquer), Ladino (Assassino, Ladrão), Mago (qualquer)</td></tr>
      </tbody>
    </table>


    <h3>Classes e Subclasses Permitidas</h3>
    <table>
      <thead>
        <tr><th>Classe</th><th>Subclasse</th></tr>
      </thead>
      <tbody>
        <tr><td>Artífice</td><td>Alquimista, Armeiro, Artilheiro, Ferreiro de Batalha</td></tr>
        <tr><td>Bárbaro</td><td>Árvore do Mundo, Berserker, Besta, Coração Selvagem, Fanático, Gigante, Guardião Ancestral, Magia Selvagem</td></tr>
        <tr><td>Bardo</td><td>Bravura, Conhecimento, Criação, Dança, Eloquência, Espadas, Glamour, Sussuros</td></tr>
        <tr><td>Bruxo</td><td>Arquifada, Celestial, Gênio, Grande Antigo, Imortal, Ínfero, Insondável, Má-Lâmina</td></tr>
        <tr><td>Clérigo</td><td>Arcana, Conhecimento, Forja, Guerra, Luz, Morte, Natureza, Ordem, Paz, Trapaça, Tempestade, Vida</td></tr>
        <tr><td>Druida</td><td>Esporos, Estrelas, Fogo Selvagem, Lua, Mar, Pastoreio, Sonhos, Terra </td></tr>
        <tr><td>Feiticeiro</td><td>Aberrante, Alma Divina, Dracônico, Feitiçaria da Tormenta, Feitiçaria Selvagem, Magia Sombria, Mecânico</td></tr>
        <tr><td>Guardião</td><td>Andarilho do Horizonte, Andarilho Feérico, Caçador, Drakewarden, Guardião do Enxame, Matador de Monstros, Senhor das Feras, Vigilante das Sombras</td></tr>
        <tr><td>Guerreiro</td><td>Arqueiro Arcano, Campeão, Cavaleiro, Cavaleiro Místico, Combatente Psíquico, Mestre de Batalha, Porta Estandarte, Samurai</td></tr>
        <tr><td>Ladino</td><td>Adaga Espiritual, Assassino, Batedor, Bucaneiro, Inquisitivo, Ladrão, Malfeitor, Trapaceiro Arcano</td></tr>
        <tr><td>Mago</td><td>Abjurador, Adivinhador, Convocador, Encantador, Evocador, Ilusionista, Necromante, Transmutador, Magia de Guerra, Ordem dos Escribas</td></tr>
        <tr><td>Monge</td><td>Dragão Ascendido, Elementos, Kensei, Mão Espalmada, Mestre Bêbado, Misericórdia, Projeção Astral, Sombras</td></tr>
        <tr><td>Paladino</td><td>Anciões, Coroa, Conquista, Devoção, Glória, Quebrador de Juramentos, Redenção, Vingança</td></tr>
      </tbody>
    </table>
    

    <h3>Equipamento Inicial</h3>
    <p>
      Seu equipamento inicial consiste nos itens de origem e o dinheiro inicial do seu nível que varia de acordo com o cenário:
    </p>
    <table>
      <thead>
        <tr>
          <th>Nível</th>
          <th>Padrão Ouro (po)</th>
          <th>Padrão Crédito ($)</th>
          <th>Padrão Prata (pp/po/pl)</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>1</td><td>100</td><td>100,00</td><td>100 pp</td></tr>
        <tr><td>2</td><td>200</td><td>200,00</td><td>200 pp</td></tr>
        <tr><td>3</td><td>300</td><td>300,00</td><td>300 pp</td></tr>
        <tr><td>4</td><td>500</td><td>500,00</td><td>500 pp</td></tr>
        <tr><td>5</td><td>800</td><td>800,00</td><td>800 pp</td></tr>
        <tr><td>6</td><td>3.000</td><td>3.000,00</td><td>30 po</td></tr>
        <tr><td>7</td><td>5.000</td><td>5.000,00</td><td>50 po</td></tr>
        <tr><td>8</td><td>7.000</td><td>7.000,00</td><td>70 po</td></tr>
        <tr><td>9</td><td>10.000</td><td>10.000,00</td><td>100 po</td></tr>
        <tr><td>10</td><td>13.000</td><td>13.000,00</td><td>130 po</td></tr>
        <tr><td>11</td><td>19.000</td><td>19.000,00</td><td>190 po</td></tr>
        <tr><td>12</td><td>27.000</td><td>27.000,00</td><td>270 po</td></tr>
        <tr><td>13</td><td>36.000</td><td>36.000,00</td><td>360 po</td></tr>
        <tr><td>14</td><td>49.000</td><td>49.000,00</td><td>490 po</td></tr>
        <tr><td>15</td><td>66.000</td><td>66.000,00</td><td>660 po</td></tr>
        <tr><td>16</td><td>88.000</td><td>88.000,00</td><td>880 po</td></tr>
        <tr><td>17</td><td>110.000</td><td>110.000,00</td><td>11 pl</td></tr>
        <tr><td>18</td><td>150.000</td><td>150.000,00</td><td>15 pl</td></tr>
        <tr><td>19</td><td>200.000</td><td>200.000,00</td><td>20 pl</td></tr>
        <tr><td>20</td><td>260.000</td><td>260.000,00</td><td>26 pl</td></tr>
      </tbody>
    </table>

<h2>MANA (Opcional)</h2>
<p>
  Em vez de espaços de magia tradicionais, conjuradores em Auramana podem utilizar o poder fluido e invisível chamado <strong>Mana</strong>. A quantidade de Mana disponível, representada como <em>Pontos de Mana</em> ou <em>Piscina de Mana</em> (PM), é determinada pelo nível e pela natureza da classe conjuradora.
 
</p>

<p>
  Caso você utilize a mecânica de mana, você fica sujeito ao <strong>Tabu da Magia</strong>.
</p>

<h3>Piscina de Mana</h3>
<div class='classTable'>
  <table>
    <thead>
      <tr>
        <th>Nível</th>
        <th>Bardo, Clérigo, Druida, Mago, Feiticeiro</th>
        <th>Guardião, Paladino</th>
        <th>Cavaleiro Místico e Trapaceiro Arcano</th>
        <th>Bruxo</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>1º</td><td>4</td><td>2</td><td>0</td><td>2</td></tr>
      <tr><td>2º</td><td>6</td><td>4</td><td>0</td><td>4</td></tr>
      <tr><td>3º</td><td>14</td><td>6</td><td>4</td><td>6</td></tr>
      <tr><td>4º</td><td>18</td><td>6</td><td>6</td><td>6</td></tr>
      <tr><td>5º</td><td>28</td><td>14</td><td>6</td><td>10</td></tr>
      <tr><td>6º</td><td>32</td><td>14</td><td>6</td><td>10</td></tr>
      <tr><td>7º</td><td>38</td><td>18</td><td>14</td><td>12</td></tr>
      <tr><td>8º</td><td>44</td><td>18</td><td>14</td><td>12</td></tr>
      <tr><td>9º</td><td>58</td><td>28</td><td>14</td><td>14</td></tr>
      <tr><td>10º</td><td>64</td><td>28</td><td>18</td><td>14</td></tr>
      <tr><td>11º</td><td>74</td><td>32</td><td>18</td><td>22</td></tr>
      <tr><td>12º</td><td>74</td><td>32</td><td>18</td><td>22</td></tr>
      <tr><td>13º</td><td>84</td><td>38</td><td>28</td><td>22</td></tr>
      <tr><td>14º</td><td>84</td><td>38</td><td>28</td><td>22</td></tr>
      <tr><td>15º</td><td>94</td><td>44</td><td>28</td><td>22</td></tr>
      <tr><td>16º</td><td>94</td><td>44</td><td>32</td><td>22</td></tr>
      <tr><td>17º</td><td>108</td><td>58</td><td>32</td><td>28</td></tr>
      <tr><td>18º</td><td>114</td><td>58</td><td>32</td><td>28</td></tr>
      <tr><td>19º</td><td>124</td><td>64</td><td>38</td><td>28</td></tr>
      <tr><td>20º</td><td>134</td><td>64</td><td>38</td><td>28</td></tr>
    </tbody>
  </table>
</div>

<h3>Custo de Mana por Magia</h3>
<p>O custo de conjurar uma magia em Auramana é determinado pelo círculo escolhido. O valor de PM é sempre o dobro do nível da magia.</p>
<table>
  <thead>
    <tr><th>Círculo</th><th>Custo (PM)</th></tr>
  </thead>
  <tbody>
    <tr><td>1º</td><td>2</td></tr>
    <tr><td>2º</td><td>4</td></tr>
    <tr><td>3º</td><td>6</td></tr>
    <tr><td>4º</td><td>8</td></tr>
    <tr><td>5º</td><td>10</td></tr>
    <tr><td>6º</td><td>12</td></tr>
    <tr><td>7º</td><td>14</td></tr>
    <tr><td>8º</td><td>16</td></tr>
    <tr><td>9º</td><td>18</td></tr>
  </tbody>
</table>
<p><em>Exemplo:</em> conjurar <strong>Curar Ferimentos</strong> no 1º círculo custa 2 PM. Se for conjurada como magia de 3º círculo, o custo sobe para 6 PM; no 7º círculo, 14 PM.</p>

<h3>Tabu da Magia (Opcional)</h3>
<p>
  Em Auramana, magia é poder, mas também é risco. Quando um conjurador utiliza mais de uma magia de 6º círculo ou superior por dia, deve desafiar os próprios limites da realidade e rolar um d20 na <strong>Tabela do Tabu</strong>.
</p>

<h4>Tabela do Tabu</h4>
<table>
  <thead>
    <tr><th>Resultado (d20)</th><th>Efeito</th></tr>
  </thead>
  <tbody>
    <tr><td>17–20</td><td>Nada acontece</td></tr>
    <tr><td>6–16</td><td>Magia Implode</td></tr>
    <tr><td>1–5</td><td>Deflagração de Mana</td></tr>
  </tbody>
</table>

<h4>Magias Implodidas</h4>
<p>A magia falha de forma abrupta. Toda energia acumulada se dissipa, e o conjurador perde os PM gastos sem nenhum efeito.</p>

<h4>Deflagração de Mana</h4>
<p>
  A magia explode em uma onda caótica de energia. Criaturas e objetos num raio de 9 metros do conjurador sofrem 5 de dano de <strong>Força</strong> por cada PM gasto. Uma salvaguarda de Constituição (CD 10 + círculo da magia) reduz o dano pela metade.
</p>
<p>
  Caso o resultado na Tabela do Tabu seja <strong>1</strong>, todos na área falham automaticamente na salvaguarda.
</p>

<h3>Dupla Concentração</h3>
<p>
  A partir do 8º nível, conjuradores plenos (bardo, bruxo, clérigo, druida, mago e feiticeiro) podem trocar uma Melhoria de Atributo pelo talento <strong>Dupla Concentração</strong>.
</p>
<p>
  Este talento permite manter <em>duas magias de concentração</em> simultaneamente. Manter a primeira magia requer uma ação bônus por turno. Manter duas requer uma ação bônus <strong>e</strong> o gasto de 2 PM por rodada.
</p>
<p>
  Sempre que sofrer dano, o conjurador deve realizar <strong>dois testes de Constituição</strong> para manter ambas as concentrações.
</p>


<div class="wide">
  <h2>RAÇAS</h2>
</div>

<section class="raca">
  <h3>Humano</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Os humanos atingem a idade adulta no final da adolescência e vivem menos de um século.</li>
    <li><strong>Tamanho:</strong> Médio (entre 1,5m e 1,8m).</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Dois idiomas à escolha.</li>
    <li><strong>Perícia:</strong> Proficiência em uma perícia à escolha.</li>
    <li><strong>Talento:</strong> Um talento à sua escolha.</li>
  </ul>
</section>

<section class="raca">
  <h3>Anjo / Demônio</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Igual à humana.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever três idiomas, sendo um deles preferencialmente um idioma antigo (latim, sumério, azteca, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Asas:</strong> Com uma ação bônus, você pode fazer um par de asas brotar ou sumir de suas costas. Você recebe deslocamento de vôo, em metros, igual a 3 vezes seu bônus de proficiência.</li>
    <li><strong>Resistência Elemental:</strong> Você recebe resistência a dano ígneo. Além disto, escolha entre dano radiante ou necrótico. Você recebe resistência ao dano escolhido e vulnerabilidade ao outro.</li>
  </ul>
</section>

<section class="raca">
  <h3>Feérico</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Variável.</li>
    <li><strong>Tamanho:</strong> Médio (na forma humana).</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever dois idiomas, sendo um deles relacionados à sua origem feérica (irlandês, coreano, iorubá, polonês, árabe, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Aparência Feérica:</strong> Você possui uma aparência humana e uma aparência feérica. Escolha uma das aparências abaixo. Uma vez feita a escolha, ela não pode ser alterada. Você pode usar uma ação bônus para se transformar e receber características de sua aparência. Seu equipamento mundano some enquanto transformado.</li>
  </ul>
  <h4>Aparências Feéricas</h4>
  <p>Escolha uma das aparências  feéricas e os benefícios que ela concede enquanto estiver transformado.</p>
  <p>A aparência feérica geralmente consiste em orelhas pontudas, mudança na tonalidade de pele e cabelo, porém algumas aparências possuem aspectos animais, como orelhas, cascos e caudas.</p>
  <p>Escolha uma das formas abaixo:</p>
  <ul>
    <li><strong>Duende:</strong> Seu tamanho muda para pequeno e você recebe acesso a um poder de origem (uma vez feita a escolha do poder, ela não pode ser alterada).</li>
    <li><strong>Elfo:</strong> Escolha duas perícias entre Acrobacia, Arcanismo, Atuação, Furtividade, Percepção, Persuasão e Sobrevivência. Você rola com vantagem os testes das perícias escolhidas enquanto estiver na forma feérica. </li>
    <li><strong>Fada:</strong> Seu tamanho muda para pequeno e um par de asas brotam de suas costas. Você recebe -2 em Força e deslocamento de Voo de 9m.</li>
    <li><strong>Jin:</strong> Você recebe resistência a dano ígneo e caso receba novamente esta resistência, ela se torna imunidade. Além disto, você pode gastar sua ação bônus ou reação para fazer com que um aliado em alcance de 9m role seu próximo teste com vantagem. O aliado precisa gastar uma ação bônus ou reação pedindo seu auxílio. Você só pode usar esta habilidade três vezes e recupera os usos após um descanso longo.</li>
    <li><strong>Ogro:</strong> Você recebe tamanho grande, +2 em Força e Constituição e -2 em Destreza.</li>
    <li><strong>Yokai:</strong> Escolha um tamanho entre pequeno, médio ou grande. Uma vez feita esta escolha, ela não pode ser alterada. Escolha também um poder de origem. Ao se transformar, você fica com o tamanho de sua aparência feérica e ganha acesso ao poder escolhido.</li>
  </ul>
</section>


<section class="raca">
  <h3>Lobisomem</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Igual à humana.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Dois idiomas à escolha.</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Armas Naturais:</strong> Seus ataques desarmados causam 1d6 + Força de dano cortante ou perfurante. Seus ataques desarmados são considerados mágico.</li>
    <li><strong>Forma Animal:</strong> Escolha um animal de CR 1 ou menor. De preferência, um mamífero predador (lobo atroz, leão, tigre, hiena gigante, urso pardo, etc). Uma vez feita a escolha, ela não pode ser alterada. Com uma ação bônus, você pode pode ficar nna forma escolhida uma quantidade horas iguais ao seu bônus de proficiência. As regras de transformação são similares à Forma Selvagem do Druida.</li>
    <li><strong>Sensibilidade à Prata:</strong> Armas banhadas em prata ignoram suas resistências que você possua e os PV temporários de sua Forma Animal.</li>
  </ul>
</section>

<section class="raca">
  <h3>Monstro</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Variável.</li>
    <li><strong>Tamanho:</strong> Médio (na forma humana).</li>
    <li><strong>Velocidade:</strong> 9 metros (na forma humana).</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever dois idiomas, sendo um deles relacionados à sua origem primordial (grego, chinês, norueguês, aimará, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Forma Primordial:</strong>  Você possui uma aparência humana e uma forma primordial. Escolha uma das formas abaixo. Uma vez feita a escolha, ela não pode ser alterada. Você pode usar uma ação bônus para se transformar e receber características de sua forma primordial. Seu equipamento mundano some enquanto transformado.</li>
  </ul>
  <h4>Formas Primordiais</h4>
  <ul>
    <li><strong>Dragão:</strong> Escolha um truque de Evocação que funciona como seu sopro e um tamanho de pequeno a grande (uma vez feita estas escolhas, não podem ser alteradas). Seu atributo de conjuração para o sopro é Constituição (caso possua um atributo mental com valor superior, pode utilizá-lo para conjuração). Você também recebe deslocamento de vôo, em metros, igual a 3 vezes seu bônus de proficiência, resistência a um dano elemental e vulnerabilidade a um dano elemental.</li>
    <li><strong>Goblin:</strong> Seu tamanho muda para pequeno e você recebe acesso a um poder de origem (uma vez feita a escolha do poder, ela não pode ser alterada).</li>
    <li><strong>Golem:</strong> Como construto, magias como Curar Ferimentos não afetam você. Você é imune a dano de veneno, ser envenenado, doenças e à exaustão. Você não precisa comer ou respirar enquanto transformado. Em vez de dormir, você entra em um estado inativo por 6 horas por dia. Você não sonha neste estado; você está totalmente ciente de seus arredores e percebe inimigos se aproximando e outros eventos normalmente. A magia Reparar o estabiliza como  truque e pode ser conjurada em você como a magia Curar Ferimentos gastando os recursos necessários por círculo de magia.</li>
    <li><strong>Górgona:</strong> Com uma ação, você pode fazer com que um alvo em alcance de 9 metros faça uma salvaguarda de Constituição (DC igual  8 + bônus de proficiência + seu modificador de Constituição). Em um teste de resistência falho, a criatura começa a se transformar em pedra e fica **restringida**. A criatura restringida deve repetir o teste de resistência no final de seu próximo turno, ficando **petrificada** em caso de falha ou encerrando o efeito em caso de sucesso. A petrificação dura 1 minuto ou até que a criatura seja libertada pela magia Restauração Maior ou outra magia similar. A menos que seja surpreendida, uma criatura pode desviar o olhar para evitar o teste de resistência no início de seu turno. Se a criatura fizer isso, ela não poderá vê-lo até o início do próximo turno, quando poderá desviar o olhar novamente. Se a criatura olhar para você nesse meio tempo, ela deve fazer o teste imediatamente. Você pode usar esta habilidade apenas uma vez no mesmo alvo a cada dia.</li>
    <li><strong>Gigante:</strong> Você recebe tamanho grande, +2 em Força, -2 em Destreza e uma quantidade de PV extras iguais a quatro vezes o seu bônus de proficiência.</li>
    <li><strong>Tritão:</strong> Você recebe deslocamento de natação, em metros, igual a quatro vezes seu bônus de proficiencia e pode respirar de baixo d'água.</li>
  </ul>
</section>


<section class="raca">
  <h3>Múmia</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Não envelhece.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong>  Você pode falar, ler e escrever três idiomas, sendo um deles preferencialmente um idioma antigo (egípcio antigo, chinês antigo, azteca, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Natureza Morta-Viva:</strong> Você não precisa respirar, é imune a dano necrótico e venenoso e à exaustão. Porém é vulnerável a dano ígneo e radiante, além de não se beneficiar de magias de cura (considerado dano radiante). Além disto, você não precisa fazer salvaguardas de morte quando chega a 0 PV, porém seu corpo é destruído se continuar sofrendo dano.</li>
    <li><strong>Resistência:</strong> Você possui resistência a dano cortante, contundente e perfurante de fontes não mágicas. Armas banhadas em prata ignoram suas resistências a dano.</li>
  </ul>
</section>

<section class="raca">
  <h3>Vampiro</h3>
  <hr>
  <ul>
    <li><strong>Idade:</strong> Não envelhece.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> Sua velocidade básica de caminhada é de 9 metros e aumenta +1,5m sempre que seu bônus de proficiência aumenta. Sua velocidade de escalada é de 9 metros.</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever três idiomas, sendo um deles preferencialmente um idioma antigo (latim, sumério, azteca, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Natureza Morta-Viva:</strong> Você não precisa respirar, é imune a dano necrótico e venenoso e à exaustão. Porém é vulnerável a dano ígneo e radiante, além de não se beneficiar de magias de cura (considerado dano radiante). Além disto, você não precisa fazer salvaguardas de morte quando chega a 0 PV, porém seu corpo é destruído se continuar sofrendo dano.</li>
    <li><strong>Resistência:</strong> Você possui resistência a dano cortante, contundente e perfurante de fontes não mágicas. Armas banhadas em prata ignoram suas resistências a dano.</li>
    <li><strong>Sono Diurno:</strong> Enquanto estiver de dia, você precisa passar oito horas no subterrâneo ou num lugar escuro (como num caixão). Você fica inconsciente e indefeso enquanto isso, em estado de torpor. Se fizer isso, recupera PV e PM (ou espaços de magia) por descanso. Caso contrário, sofre os efeitos de fome.</li>
    <li><strong>Sensibilidade à Luz:</strong> Você sofre uma quantidade de dano radiante igual o dobro de seu bônus de proficiência ao iniciar seu turno sob a luz solar (já contabilizada a sua vulnerabilidade). Enquanto estiver sob a luz solar, também tem desvantagem em jogadas de ataque e testes de perícia.</li>
  </ul>
  <h4>Sede de Sangue</h4>
    <p>
      Diferente de outros mortos-vivos, os vampiros sentem uma fome voraz por sangue. Isto lhe concede as seguintes características:
    </p>

  <ul>
    <li>Você pode drenar sangue e energia vital de uma criatura disposta, ou de uma que esteja agarrada, incapacitada ou restringida por você. Faça um teste de agarrar utilizando Força (Atletismo) contra o alvo. Caso tenha sucesso, pode usar sua ação bônus para fazer um ataque com sua mordida. Se acertar, você causa 1d4 de dano perfurante + uma quantidade de dano necrótico igual ao seu bônus de proficiência. Você recupera pontos de vida equivalentes ao dano causado. Você não pode recuperar pontos de vida de alvos que não possuem sangue (como construtos ou espectros).</li>
    <li> Ficar sem beber pelo menos um gole de sangue por dia causa efeitos de fome (um vampiro pode ficar sem beber sangue por um número de dias igual a 3 + seu modificador de Constituição - mínimo 1 dia. Ao final de cada dia que ultrapassar esse limite, o vampiro sofrerá automaticamente um nível de exaustão. Um dia normal de alimentação zera a contagem de dias sem comida.</li>
  </ul>
</section>

  </div>

</body>
</html>
