<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <title>Arcanista</title>
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

        h1,
        h2 {
            text-align: center;
            color: var(--cor-texto);
            text-shadow: 1px 1px var(--cor-destaque);
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

<div class="classe">
  <h1>Arcanista</h1>
</div>

<p>Mestres da magia que dominam os segredos arcanos através de estudo, tradição ou poder inato></p>

<p>Os arquétipos de arcanista são Bruxo, Feiticeiro, Mago e Necromente</p>


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


<h2>Tabela de Progressão</h2>

<table class="progressao-arcanista">
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
    <tr>
      <td>6</td>
      <td>Poder de Arcanista</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Arquétipo Arcano</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Aumento de Atributo</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Magias (3º Círculo), Raio Poderoso, Raio Arcano (3d12)</td>
    </tr>
    <tr>
      <td>10</td>
      <td>Poder de Arcanista</td>
    </tr>
    <tr>
      <td>11</td>
      <td>Arquétipo Arcano</td>
    </tr>
    <tr>
      <td>12</td>
      <td>Aumento de Atributo</td>
    </tr>
    <tr>
      <td>13</td>
      <td>Magias (4º Círculo), Raio Arcano (4d12), Fluxo de Mana</td>
    </tr>
    <tr>
      <td>14</td>
      <td>Poder de Arcanista</td>
    </tr>
    <tr>
      <td>15</td>
      <td>Arquétipo Arcano</td>
    </tr>
    <tr>
      <td>16</td>
      <td>Aumento de Atributo</td>
    </tr>
    <tr>
      <td>17</td>
      <td>Magias (5º Círculo), Raio Arcano (5d12), Magia Ilimitada</td>
    </tr>
    <tr>
      <td>18</td>
      <td>Poder de Arcanista</td>
    </tr>
    <tr>
      <td>19</td>
      <td>Aumento de Atributo</td>
    </tr>
    <tr>
      <td>20</td>
      <td>Alta Arcana, Poder de Arcanista</td>
    </tr>
  </tbody>
</table>


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

<div class="habilidade">
  <h3>Fortalecimento Arcano</h3>
  <p>A CD para resistir a suas magias aumenta em +1. Se você puder lançar magias de 4º círculo, em vez disso ela aumenta em +2.</p>
</div>

<div class="habilidade">
  <h3>Raio Poderoso</h3>
  <p>Os dados de dano do seu Raio Arcano aumentam para d12 e o alcance dele aumenta para médio. Pré-requisito: Raio Arcano.</p>
</div>

<div class="habilidade">
  <h3>Fluxo de Mana</h3>
  <p>Você pode manter dois efeitos sustentados ativos simultaneamente com apenas uma ação livre, pagando o custo de cada efeito separadamente.</p>
</div>

<div class="habilidade">
  <h3>Magia Ilimitada</h3>
  <p>Você soma seu atributo-chave no limite de PM que pode gastar numa magia. Por exemplo, um arcanista de 17º nível com Int 6 e este poder pode gastar até 23 PM em cada magia. Utilização deste poder causar áreas de Corrupção e o Tabu da Magia.</p>
</div>

<div class="habilidade">
  <h3>Alta Arcana</h3>
  <p>No 20º nível, você deixa de ser afetado pelo Tabu da Magia. Além disso, o custo básico de suas magias cai para 2 PM (2º círculo), 3 PM (3º círculo), 4 PM (4º círculo) e 5 PM (5º círculo).</p>
</div>

<div class="habilidade">
  <h3>Aumento de Atributo</h3>
  <p>Você recebe +1 em um atributo, porém não pode escolher o mesmo atributo duas vezes seguidas. Você pode substituir este aumento de atributo por um poder geral.</p>
</div>

<div class="habilidade">
  <h3>Arquétipo Arcano</h3>
  <p>Escolha um dos arquétipos arcanos entre Bruxo, Feiticeiro e Mago. Você recebe as habilidades relacionadas a estes arquétipos em determinados níveis.</p>
</div>

<div class="habilidade">
  <h3>Poder de Arcanista</h3>
  <p>Você recebe um poder de arcanista.</p>
</div>

<h2 id="arquétipos">Arquétipos Arcanos</h2>

<div class="archetype-card">
  <h3>Bruxo</h3>
  <p><em>Arcanistas que retiram seus poderes de itens, maldições e poções.</em></p>

  <div class="archetype-ability">
    <h4>1º Nível: Foco Arcano</h4>
    <p>Você lança magias através de um foco (varinha, cajado, chapéu...). Para lançar magias:</p>
    <ul>
      <li>Deve empunhar o foco com uma mão e gesticular com a outra</li>
      <li>Ou fazer teste de Misticismo (CD 20 + custo em PM da magia)</li>
      <li><strong>Falha:</strong> Gasta metade dos PM (mínimo 1) e não lança a magia</li>
    </ul>
    <p><strong>Características do Foco:</strong></p>
    <ul>
      <li>RD 10 e PV = metade dos seus PV</li>
      <li>Restaurado completamente ao recuperar PM</li>
      <li>Destruído (0 PV): Fica Frustrado por 1d4-1 rodadas</li>
      <li>Pode ser recuperado com 1 semana de trabalho e 100 PP</li>
    </ul>
    <p><strong>Atributo de Conjuração:</strong> Sabedoria (usa Sab para Misticismo e Ofício Alquimia)</p>
  </div>

  <div class="archetype-ability">
    <h4>3º Nível: Familiar</h4>
    <p>Adquire um animal de estimação mágico do tipo familiar com habilidades especiais.</p>
    <p><strong>Bônus:</strong> Torna-se treinado em Ofício (Alquimia) se não for</p>
  </div>

  <div class="archetype-ability">
    <h4>7º Nível: Caldeirão do Bruxo</h4>
    <p>Pode criar poções como com o poder <em>Preparar Poção</em>:</p>
    <ul>
      <li>Se já tiver o poder, pode criar poções de até 5º círculo</li>
      <li>Poções criadas têm efeito mais potente</li>
    </ul>
  </div>

  <div class="archetype-ability">
    <h4>11º Nível: Praguejar</h4>
    <p><strong>Custo:</strong> 2 PM</p>
    <p>Força um adversário a rerrolar um teste recém realizado.</p>
    <p><strong>Limitação:</strong> 1 vez por cena por adversário</p>
  </div>

  <div class="archetype-ability">
    <h4>15º Nível: Maldição</h4>
    <p>Aprende a magia <em>Rogar Maldição</em> e pode simular efeitos de outras magias:</p>
    <ul>
      <li>Magias simuláveis: Alterar Tamanho, Amedrontar, Apagar Memória, etc.</li>
      <li>Custo extra igual ao custo da magia simulada</li>
      <li>Se aprender a magia original: redução de PM igual ao círculo</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo:</strong> Simular <em>Alterar Tamanho</em> com aprimoramento para minúsculo:</p>
      <p>Rogar Maldição (3 PM) + Efeito (3 PM) + Aprimoramento (7 PM) = 13 PM total</p>
      <p>Se aprender <em>Alterar Tamanho</em>: custo reduz para 10 PM (13 - 3)</p>
    </div>
  </div>
</div>


<div class="archetype-card">
  <h3>Feiticeiro</h3>
  <p><em>Portadores de magia inata, cujos poderes fluem através de linhagens sobrenaturais</em></p>

  <div class="archetype-ability">
    <h4>1º Nível: Herança Mágica</h4>
    <p>Sua magia surge de uma linhagem sobrenatural em seu sangue:</p>
    <ul>
      <li>Escolha uma linhagem (dragônica, elemental, feérica, etc.)</li>
      <li>Recebe a <strong>herança básica</strong> da linhagem escolhida</li>
      <li>Não depende de itens ou estudo para conjurar</li>
      <li><strong>Aprendizado limitado:</strong> Nova magia a cada nível ímpar (3º, 5º...)</li>
    </ul>
    <p><strong>Atributo de Conjuração:</strong> Carisma (usa Car para Misticismo)</p>
  </div>

  <div class="archetype-ability">
    <h4>3º Nível: Metamagia</h4>
    <p>Escolha um dos seguintes poderes mágicos:</p>
    <ul class="power-list">
      <li><strong>Geometria Mística:</strong> Modifica área de efeito das magias</li>
      <li><strong>Magia Acelerada:</strong> Conjuração como ação livre (1x/cena)</li>
      <li><strong>Magia Ampliada:</strong> Aumenta alcance das magias</li>
      <li><strong>Magia Discreta:</strong> Conjuração silenciosa e sutil</li>
    </ul>
    <p><strong>Força de Vontade:</strong> Usa Carisma em testes de Vontade</p>
  </div>

  <div class="archetype-ability">
    <h4>7º Nível: Herança Aprimorada</h4>
    <p>Desbloqueia poderes avançados de sua linhagem:</p>
    <ul>
      <li>Efeitos passivos constantes</li>
      <li>Habilidades ativas únicas</li>
      <li>Resistências a tipos específicos de dano</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo (Linhagem Dragônica):</strong> Asas vestigiais, resistência a um tipo de dano, sopro elemental</p>
    </div>
  </div>

  <div class="archetype-ability">
    <h4>11º Nível: Herança Superior</h4>
    <p>Manifestação poderosa de sua linhagem:</p>
    <ul>
      <li>Transformações parciais</li>
      <li>Aprimoramento de habilidades anteriores</li>
      <li>Novas capacidades ofensivas/defensivas</li>
    </ul>
  </div>

  <div class="archetype-ability">
    <h4>15º Nível: Apoteose</h4>
    <p>Ápice de sua herança sobrenatural:</p>
    <ul>
      <li>Forma verdadeira da linhagem</li>
      <li>Poderes equivalentes a magias de 5º círculo</li>
      <li>Mudanças permanentes em sua fisiologia</li>
      <li>Habilidade única definitiva</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo (Linhagem Infernal):</strong> Asas de demônio, imunidade a fogo, aura de medo</p>
    </div>
  </div>
</div>

<div class="lineage-details">
  <h5>Linhagem Dragônica</h5>
  <p>Descrição dos poderes...</p>
</div>


<div class="archetype-card">
  <h3>Mago</h3>
  <p><em>Eruditos que dominam a magia através de estudo metódico e memorização precisa</em></p>

  <div class="archetype-ability">
    <h4>1º Nível: Grimório</h4>
    <p>Sua magia depende de estudo e memorização:</p>
    <ul>
      <li>Só pode lançar magias <strong>memorizadas</strong></li>
      <li><strong>Memorização:</strong> 1h de estudo para memorizar metade das magias conhecidas</li>
      <li>Pode rememorizar 1x/dia (requer grimório)</li>
      <li><strong>Grimório:</strong> Mesmas estatísticas que foco de bruxo (RD 10, PV = metade dos seus)</li>
      <li><strong>Bônus:</strong> +1 magia inicial e +1 magia por novo círculo</li>
    </ul>
    <p><strong>Atributo de Conjuração:</strong> Inteligência (usa Int para Vontade)</p>
  </div>

  <div class="archetype-ability">
    <h4>3º Nível: Escriba Arcano</h4>
    <ul>
      <li>Torna-se treinado em <strong>Ofício (Escriba)</strong></li>
      <li>Pode copiar magias de outros grimórios/pergaminhos</li>
      <li><strong>Custo:</strong> 1 dia + 200 PP por PM da magia</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo:</strong> Aprender magia de 3º círculo (6 PM):</p>
      <p>6 dias + 1.200 PP</p>
    </div>
  </div>

  <div class="archetype-ability">
    <h4>7º Nível: Tinta do Mago</h4>
    <p>Domínio da criação de pergaminhos:</p>
    <ul>
      <li>Ganha habilidade de <strong>Escrever Pergaminho</strong></li>
      <li>Se já tiver o poder: custo de criação reduzido pela metade</li>
      <li>Pergaminhos criados são mais resistentes</li>
    </ul>
  </div>

  <div class="archetype-ability">
    <h4>11º Nível: Geometria Mística</h4>
    <p>Controle preciso sobre magias de área:</p>
    <ul>
      <li>Pode excluir <strong>Inteligência</strong> alvos dos efeitos</li>
      <li>Não requer teste ou custo adicional</li>
      <li>Combina com outras metamágias</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo:</strong> Int 5 → Exclui 5 aliados de uma magia de bola de fogo</p>
    </div>
  </div>

  <div class="archetype-ability">
    <h4>15º Nível: Arquimago</h4>
    <p>Domínio sobre magias divinas:</p>
    <ul>
      <li>Pode aprender magias divinas de textos sagrados</li>
      <li><strong>Custo:</strong> Triplo de tempo e recursos</li>
      <li>Limite de círculo igual ao seu círculo arcano máximo</li>
    </ul>
    <div class="example">
      <p><strong>Exemplo:</strong> Aprender <em>Cura Moderada</em> (2º círculo divino):</p>
      <p>6 dias + 1.800 PP (vs 2 dias + 600 PP para magia arcana)</p>
    </div>
  </div>
</div>


<div class="archetype-card">
  <h3>Necromante</h3>
  <p><em>Mestres das artes sombrias que manipulam as energias da morte e dos mortos</em></p>

  <div class="archetype-ability">
    <h4>1º Nível: Necrologia</h4>
    <p>Você lança magias através de sua conexão com a morte:</p>
    <ul>
      <li>Todas as magias que você aprende devem ser de necromancia, arcanas ou divinas</li>
      <li>Recebe <strong>+1 em Cura, Fortitude</strong> e na <strong>CD de magias de Necromancia</strong></li>
      <li>Este bônus aumenta em níveis superiores</li>
    </ul>
    <p><strong>Atributo de Conjuração:</strong> Inteligência (usa Int para Vontade e Cura no lugar de Sab)</p>
  </div>

  <div class="archetype-ability">
    <h4>3º Nível: Distorção Necrótica</h4>
    <ul>
      <li>A cada nível ímpar a partir do 3º, pode aprender uma magia de outra escola como se fosse de necromancia</li>
      <li>Magias do poder Conhecimento Mágico também podem ser distorcidas</li>
      <li>Efeitos visuais mudam para temas necróticos (ex: armadura de ossos, chamas verdes, asas cadavéricas)</li>
    </ul>
    <h5>Especialista em Necromancia</h5>
    <p>A CD para resistir a suas magias de necromancia aumenta em <strong>+2</strong></p>
  </div>

  <div class="archetype-ability">
    <h4>7º Nível: Animar Cadáver</h4>
    <p>Controle sobre os mortos:</p>
    <ul>
      <li><strong>Ação padrão</strong> e <strong>3 PM</strong> para animar cadáver de criatura Pequena, Média ou Grande em alcance curto</li>
      <li>Torna-se parceiro iniciante (não conta no limite de parceiros)</li>
      <li>Pode sacrificar o parceiro para reduzir dano recebido à metade</li>
      <li>Limite: 1 parceiro cadáver por vez</li>
    </ul>
    <p><strong>Necrologia:</strong> Bônus aumenta para <strong>+2</strong></p>
  </div>

  <div class="archetype-ability">
    <h4>11º Nível: Mestre Necromante</h4>
    <p>Maior eficiência em magias da morte:</p>
    <ul>
      <li>Custo para lançar magias de necromancia diminui em <strong>-1 PM</strong></li>
      <li>Cumulativo com outras reduções de custo</li>
    </ul>
  </div>

  <div class="archetype-ability">
    <h4>15º Nível: Domínio Sobre a Morte</h4>
    <p>Controle absoluto sobre cadáveres:</p>
    <ul>
      <li><strong>Animar Cadáver</strong> melhora:</li>
      <li>Ação livre (antes: padrão)</li>
      <li>Alcance médio (antes: curto)</li>
      <li>Alvo até Colossal (antes: Grande)</li>
      <li>Parceiro veterano (antes: iniciante)</li>
    </ul>
    <p><strong>Necrologia:</strong> Bônus aumenta para <strong>+3</strong></p>
  </div>
</div>


<style>
  .power-list {
    columns: 2;
    -webkit-columns: 2;
    -moz-columns: 2;
  }
  
  @media (max-width: 600px) {
    .power-list {
      columns: 1;
      -webkit-columns: 1;
      -moz-columns: 1;
    }
  }
</style>


<style>
.progressao-arcanista {
  width: 100%;
  border-collapse: collapse;
  margin: 20px 0;
  font-family: 'MedievalSharp', cursive;
  background-color: rgba(187, 168, 140, 0.1);
  border: 2px solid #5b4636;
}

.progressao-arcanista th {
  background-color: #5b4636;
  color: #fff9e6;
  padding: 12px;
  text-align: center;
  font-size: 1.1em;
}

.progressao-arcanista td {
  padding: 10px 15px;
  border-bottom: 1px solid #bba88c;
  vertical-align: middle;
}

.progressao-arcanista tr:nth-child(even) {
  background-color: rgba(187, 168, 140, 0.05);
}

.progressao-arcanista tr:hover {
  background-color: rgba(187, 168, 140, 0.2);
}

.progressao-arcanista td:first-child {
  font-weight: bold;
  text-align: center;
  width: 60px;
  color: #5b4636;
}

.progressao-arcanista td:nth-child(2) {
  text-align: left;
}
</style>


<style>
  .archetype-card {
    background-color: rgba(91, 70, 54, 0.1);
    border: 2px solid #5b4636;
    border-radius: 5px;
    padding: 20px;
    margin: 20px 0;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }

  .archetype-ability {
    margin-bottom: 20px;
    padding-bottom: 15px;
    border-bottom: 1px dashed #bba88c;
  }

  .archetype-ability:last-child {
    border-bottom: none;
  }

  .archetype-ability h4 {
    color: #3a2c1d;
    margin-bottom: 10px;
    font-size: 1.2em;
  }

  .example {
    background-color: rgba(187, 168, 140, 0.2);
    padding: 10px;
    border-left: 3px solid #5b4636;
    margin-top: 10px;
    font-size: 0.9em;
  }
</style>