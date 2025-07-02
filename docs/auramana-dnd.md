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
        <tr><td>Livro do Jogador (2014)</td><td>Clérigo (Conhecimento, Natureza, Tempestade), Mago (Convocador, Encantador, Necromante, Transmutador)</td></tr>
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
      Alternativamente, você pode utilizar o método de rolagem: role 4d6 e some os três maiores resultados. Faça isso seis vezes.<br>
      Em seguida, aplique os aumentos de atributos da Origem.
    </p>

    <h3>Classes e Subclasses Permitidas</h3>
        <p>
      * Além das subclasses do Modern Handbook.
    </p>
    
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
  <h2>RAÇAS (cenários modernos / dark fantasy) </h2>
</div>

<section class="raca">
  <h3>Humano</h3>
  <hr>
<p>
  O humano comum (ou nem tanto).
</p>  
  <ul>
    <li><strong>Idade:</strong> Os humanos atingem a idade adulta no final da adolescência e vivem menos de um século.</li>
    <li><strong>Tamanho:</strong> Médio (entre 1,5m e 1,8m).</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Dois idiomas à escolha.</li>
    <li><strong>Eficiente:</strong> Você adquire Inspiração Heroica sempre que completar um Descanso Longo.</li>
    <li><strong>Hábil:</strong> Proficiência em uma perícia à escolha.</li>
    <li><strong>Versátil:</strong> Um talento à sua escolha.</li>
  </ul>
</section>

<section class="raca">
  <h3>Nefelim</h3>
  <hr>
  <p>
    Encarnações de anjos e demônios. Você geralmente possui uma forma humana e esconde características demoníacas ou angelicais (cascos, cauda, chifres, múltiplos olhos, etc). Você pode esconder ou mostrar essas características com uma ação livre.  </p>  
  <ul>
    <li><strong>Idade:</strong> Igual à humana.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever três idiomas, sendo um deles preferencialmente um idioma antigo (latim, sumério, azteca, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Asas: </strong> Com uma ação bônus, um par de asas brotam de suas costas. Você recebe deslocamento de vôo, em metros, igual a 3 vezes seu bônus de proficiência.</li>
    <li><strong>Resistência Elemental:</strong> Você possui resistência a dano ígneo. Além disto, escolha entre dano radiante ou necrótico. Você possui resistência ao dano escolhido e vulnerabilidade ao outro.</li>
  </ul>
</section>

<section class="raca">
  <h3>Fábula</h3>
  <hr>
  <p>
    Todo o tipo de criatura mágica ou fantástica geralmente não alinhada entre anjos e demônios é categorizada como fábula. Fadas, gênios, dragões, yokai, gigantes, górgonas, dentre outras criaturas, são exemplos de fábulas.
  </p>  
  <ul>
    <li><strong>Idade:</strong> Variável.</li>
    <li><strong>Tamanho:</strong> Médio (na forma humana).</li>
    <li><strong>Velocidade:</strong> 9 metros (na forma humana).</li>
    <li><strong>Idiomas:</strong> Você pode falar, ler e escrever dois idiomas, sendo um deles relacionados à sua origem primordial ou feérica (irlandês, coreano, grego, chinês, iorubá, árabe, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>    
    <li><strong>Forma Fabulae:</strong> Você possui uma aparência humana e uma aparência feérica ou de monstro. Escolha uma das formas abaixo. Uma vez feita a escolha, ela não pode ser alterada. Você pode usar uma ação bônus para se transformar e receber características de sua forma não humana. Formas não humanoides, o equipamento mundano some enquanto transformado.</li>
  </ul>
  <h4>Forma Fabulae</h4>
  <ul>
    <li><strong>Anão/Gnomo:</strong> Seu tamanho muda para pequeno e você recebe deslocamento de Escavação (3m) e acesso a um poder de origem entre Crafter, Tough e Tavern Brawler (uma vez feita esta escolha, ela não pode ser alterada). Humanoide, Feérico.</li>
    <li><strong>Capuz Vermelho:</strong> Seu tamanho muda para pequeno e você rola com vantagem dtestes de Destreza (Furtividade e Ladinagem). Humanoide, Feérico.</li>    
    <li><strong>Duende/Goblin:</strong> Seu tamanho muda para pequeno e você recebe deslocamento de Escalada (6m) e acesso a um poder de origem (uma vez feita esta escolha, ela não pode ser alterada). Humanoide, Feérico.</li>    
    <li><strong>Elfo:</strong> Escolha duas perícias entre Acrobacia, Arcanismo, Atuação, Furtividade, Conhecimento Histórico, Percepção, Persuasão e Sobrevivência. Você rola com vantagem os testes de atributo relacionados às perícias escolhidas. Humanoide, Feérico.</li>
    <li><strong>Fada:</strong> Seu tamanho muda para pequeno e um par de asas brotam de suas costas. Você recebe -2 em Força e deslocamento de Voo de 9m. Feérico</li>
    <li><strong>Jinn:</strong> Você recebe resistência a um dano elemental e caso receba novamente esta resistência, ela se torna imunidade. Além disto, você pode gastar sua ação bônus ou reação para fazer com que um aliado em alcance de 9m role seu próximo teste com vantagem. O aliado precisa gastar uma ação bônus ou reação pedindo seu auxílio. Você só pode usar esta habilidade três vezes e recupera os usos após um descanso longo. Elemental, feérico.</li>
    <li><strong>Dragão:</strong> Escolha um tamanho de pequeno a grande, você muda para este tamanho e recebe deslocamento de vôo, em metros, igual a 3 vezes seu bônus de proficiência. Escolha também um truque que funciona como seu sopro entre Acid Splash, Fire Bolt, Frostbite, Infestation, Lightning Lure, Mind Sliver, Poison Spray, Ray of Frost, Sacred Flame e Toll the Dead. Seu atributo de conjuração para o sopro é Constituição (caso possua um atributo mental com valor superior, pode utilizá-lo para conjuração). Você também resistência ao dano elemental do truque escolhido e vulnerabilidade a outro dano elemental. Caso receba a resistência elemental novamente, ele se torna imunidade. Uma vez feitas estas escolhas, elas não podem ser alteradas). Monstruosidade, dragão.</li> 
    <li><strong>Ogro/Gigante:</strong> Seu tamanho muda para grande, você recebe proficiência em Atletismo (ou expertise caso já seja proficiente) e uma quantidade de PV extras iguais ao dobro de seu nível (mínimo 10 PV extras). Monstruosidade, gigante. </li>
   <li><strong>Golem:</strong> Como construto, magias como Curar Ferimentos não afetam você. Você é imune a dano de veneno, ser envenenado, doenças e à exaustão. Você não precisa comer ou respirar enquanto transformado. Em vez de dormir, você entra em um estado inativo por 6 horas por dia. Você não sonha neste estado; você está totalmente ciente de seus arredores e percebe inimigos se aproximando e outros eventos normalmente. A magia Reparar o estabiliza como truque e pode ser conjurada em você como a magia Curar Ferimentos gastando os recursos necessários por círculo de magia. Por fim, você pode substituir o talento de sua Origem pelas características de outro Fábula (por exemplo, se tornar um golem gigante ou um golem dragão), além de receber o tipo de criatura desta fábula. Construto. </li>
    <li><strong>Górgona:</strong> Com uma ação, você pode fazer com que um alvo em alcance de 9 metros faça uma salvaguarda de Constituição (DC igual  8 + bônus de proficiência + seu modificador de Constituição). Em um teste de resistência falho, a criatura começa a se transformar em pedra e fica **restringida**. A criatura restringida deve repetir o teste de resistência no final de seu próximo turno, ficando **petrificada** em caso de falha ou encerrando o efeito em caso de sucesso. A petrificação dura 1 minuto ou até que a criatura seja libertada pela magia Restauração Maior ou outra magia similar. A menos que seja surpreendida, uma criatura pode desviar o olhar para evitar o teste de resistência no início de seu turno. Se a criatura fizer isso, ela não poderá vê-lo até o início do próximo turno, quando poderá desviar o olhar novamente. Se a criatura olhar para você nesse meio tempo, ela deve fazer o teste imediatamente. Você pode usar esta habilidade apenas uma vez no mesmo alvo a cada dia. Monstuosidade, humanoide. </li>
    <li><strong>Tritão:</strong> Você pode respirar de baixo d'água e recebe deslocamento de natação de 12m, qual aumenta aumenta +1,5m sempre que seu bônus de proficiência aumenta. Monstruosidade.</li>  
    <li><strong>Undine:</strong> Você pode respirar de baixo d'água, recebe deslocamento de natação (9m) e o talento Magic Initiate (Shape Water, Create or Destroy Water e mais um truque relacionado a água). Elemental, feérico</li>  
    
  </ul>
</section>

<section class="raca">
  <h3>Licantropo</h3>
  <hr>
  <p>
    Licantropos são um tipo específico de fábula, ligados essencialmente a uma forma animal. Lobisomens, kitsunes, homens-tigres, berserkers, dentre outros, são exemplos de licantropos.
  </p>   
  <ul>
    <li><strong>Idade:</strong> Igual à humana.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong> Dois idiomas à escolha.</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Armas Naturais:</strong> Com uma ação livre, você pode entrar ou sair de uma forma híbrida entre humano e animal. Neste estado, seus ataques desarmados causam 1d6 de dano. O tipo de dano e atributo utilizado nas rolagens estão relacionados ao ataque principal de sua forma animal. Seus ataques desarmados, enquanto transformado, são considerados mágicos.</li>
    <li><strong>Forma Animal:</strong> Escolha um animal de CR 1 ou menor (lobo atroz, leão, tigre, hiena gigante, urso pardo, etc). Uma vez feita a escolha, ela não pode ser alterada. Com uma ação bônus, você pode pode ficar na forma escolhida uma quantidade horas iguais ao seu bônus de proficiência. Veja as demais regras da Forma Animal abaixo.</li>
    <li><strong>Sensibilidade à Prata:</strong> Armas banhadas em prata ignoram as resistências a dano  que você possua e os PV temporários de sua Forma Animal.</li>
  </ul>
</section>

  <h4>Forma Animal</h4>
    <p>
      Sua forma licantropa possui as seguintes características:
    </p>  
  <ul>
    <li><strong>Quantidade de Usos: </strong>Você pode usar Forma Animal quantas vezes quiser, porém o tempo máximo ao longo do dia que você pode ficar transformado é igual ao seu bônus de proficiência. Você pode sair e entrar em sua forma animal com uma ação bônus.</li>
    <li><strong>Formas Conhecidas:</strong> Você possui apenas uma forma conhecida de um animal de CR 1 ou menor. Você pode escolher uma forma que voa ou respira de baixo d'água, desde que esteja na CR indicada.</li>
    <li><strong>Estatísticas de Jogo:</strong> Suas estatísticas de jogo são substituídas pelo bloco de estatísticas da Fera, mas você mantém seu tipo de criatura, Pontos de Vida, Dados de Vida, valores de Inteligência, Sabedoria e Carisma, características de classe, idiomas e talentos. Você também mantém suas proficiências em perícia e salvaguarda e usa seu Bônus de Proficiência para elas, além de adquirir as proficiências da criatura. Se uma perícia ou modificador de salvaguarda no bloco de estatísticas da Fera for maior que o seu, use o do bloco de estatísticas.</li>
    <li><strong> Sem Conjuração:</strong> Você não pode conjurar magias, mas a multimorfia não quebra sua Concentração ou interfere em uma magia que você já conjurou.</li>
    <li><strong>Sem Pontos de Vida Temporários:</strong>  Diferente da Forma Selvagem do Druida, sua forma animal não concende pontos de vida temporário.</li>
    <li><strong> Objetos:</strong> Sua capacidade de manipular objetos é determinada pelos membros da forma, e não pelos seus. Além disso, você escolhe se seu equipamento cai em seu espaço, se funde em sua nova forma ou se é usado por ela. O equipamento vestido funciona normalmente, mas o Mestre decide se é compatível para a nova forma usar um equipamento com base no tamanho e forma da criatura. Seu equipamento não muda de tamanho ou forma para corresponder à nova forma, e qualquer equipamento que a nova forma não possa usar deve cair no chão ou se fundir com a forma. O equipamento que se funde com a forma não tem efeito enquanto você estiver nessa forma.</li>
  </ul>
</section>


<section class="raca">
  <h3>Morto-Vivo</h3>
  <hr>
  <p>
    Vampiros, múmias, zumbis e espectros são exemplos de criaturas que morreram, porém ainda vagam entre o mundo dos vivos.
  </p>  
  <ul>
    <li><strong>Idade:</strong> Não envelhece.</li>
    <li><strong>Tamanho:</strong> Médio.</li>
    <li><strong>Velocidade:</strong> 9 metros.</li>
    <li><strong>Idiomas:</strong>  Você pode falar, ler e escrever três idiomas, sendo um deles preferencialmente um idioma antigo (latim, egípcio antigo, chinês antigo, quechuá, etc).</li>
    <li><strong>Visão no Escuro:</strong> 18 metros.</li>
    <li><strong>Natureza Morta-Viva:</strong>  Você é imune a dano de veneno, ser envenenado, doenças e à exaustão. Você não precisa comer ou respirar Em vez de dormir, você deve descansar por 6 horas por dia num local escuro. Você é, porém, vulnerável a dano ígneo e radiante, além de não se beneficiar de magias de cura convencionais (causam dano radiante). Poções de cura específicas para mortos-vivos recuperam seus pontos de vida. Além disto, você não precisa fazer salvaguardas de morte quando chega a 0 PV, porém seu corpo é destruído se continuar sofrendo dano.</li>
  </ul>
  

  <h4>Vampirismo</h4>
    <p>
      Além das caractérísticas básicas de morto-vivo, vampiros recebem os seguintes tratos:
    </p>  
  <ul>
    <li><strong>Mordida: </strong>Você pode drenar sangue e energia vital de uma criatura disposta, ou de uma que esteja agarrada, incapacitada ou restringida por você. Faça um teste de agarrar utilizando Força (Atletismo) contra o alvo. Caso tenha sucesso, pode usar sua ação bônus para fazer um ataque com sua mordida. Se acertar, você causa 1d4 de dano perfurante + uma quantidade de dano necrótico igual ao seu bônus de proficiência. Você recupera pontos de vida equivalentes ao dano causado. Você não pode recuperar pontos de vida de alvos que não possuem sangue (como construtos ou espectros).</li>
    <li><strong>Sede de Sangue:</strong> Ficar sem beber pelo menos um gole de sangue por dia causa efeitos de fome (um vampiro pode ficar sem beber sangue por um número de dias igual a 3 + seu modificador de Constituição - mínimo 1 dia. Ao final de cada dia que ultrapassar esse limite, o vampiro sofrerá automaticamente um nível de exaustão. Um dia normal de alimentação zera a contagem de dias sem comida.</li>
      <li><strong>Sono Diurno:</strong> Enquanto estiver de dia, você precisa passar oito horas no subterrâneo ou num lugar escuro (como num caixão). Você fica inconsciente e indefeso enquanto isso, em estado de torpor. Se fizer isso, recupera PV e PM (ou espaços de magia) por descanso. Caso contrário, sofre os efeitos de fome.</li>
    <li><strong>Sensibilidade à Luz:</strong> Você sofre uma quantidade de dano radiante igual o dobro de seu bônus de proficiência ao iniciar seu turno sob a luz solar (já contabilizada a sua vulnerabilidade). Enquanto estiver sob a luz solar, também tem desvantagem em jogadas de ataque e testes de perícia.</li>
    <li><strong>Resistência:</strong> Você possui resistência a dano cortante, contundente e perfurante de fontes não mágicas. Armas banhadas em prata ignoram suas resistências a dano.</li>
    <li><strong>Velocidade Vampírica:</strong> Sua velocidade básica de caminhada é de 9 metros, porém aumenta +1,5m sempre que seu bônus de proficiência aumenta. Sua velocidade de escalada é de 9 metros
  </ul>
</section>

  <h4>Mumificação</h4>
    <p>
      Além das caractérísticas básicas de morto-vivo, múmias recebem os seguintes tratos:
    </p>  
  <ul>
    <li><strong>Resistência:</strong> Você possui resistência a dano cortante, contundente e perfurante de fontes não mágicas. Armas banhadas em prata ignoram suas resistências a dano.</li>
    <li><strong>Lento:</strong> Sua velocidade básica de caminhada é de 6 metros.</li>
  </ul>
</section>
  </div>

</body>
</html>
