<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <title>Raças - Auramana T20</title>
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

        .raca {
            margin-bottom: 30px;
            background-color: #f9f5f0;
            padding: 15px;
            border-radius: 5px;
            border-left: 4px solid #5b4636;
        }

        .raca h2 {
            margin-top: 0;
            color: #5b4636;
        }

        .atributos,
        .habilidades {
            margin-left: 20px;
        }

        .alternativo {
            font-style: italic;
            color: #666;
        }

        .opcao {
            font-weight: bold;
            margin-left: 15px;
        }
    </style>
</head>

<body>
    <h1>RAÇAS</h1>

    <div class="raca">
        <h2>HUMANO</h2>
        <div class="atributos">
            <p><strong>Atributos:</strong> +1 em três atributos.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em um atributo, +1 em um segundo atributo
                e -1 em um terceiro atributo.</p>
            <p><strong>PV Iniciais:</strong> +10.</p>
        </div>
        <div class="habilidades">
            <p><strong>Perito:</strong> Você se torna treinado em uma perícia à sua escolha.</p>
            <p><strong>Versátil:</strong> Você se torna em um poder geral à sua escolha ou em uma perícia. Caso você
                seja um mestiço, você pode substituir o poder geral por uma poder ou habilidade de outra raça.</p>
        </div>
    </div>

    <div class="raca">
        <h2>ANÃO</h2>
        <div class="atributos">
            <p><strong>Atributos:</strong> Constituição +1, +1 em Inteligência ou Sabedoria.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> Constituição +2, +1 em Inteligência ou
                Sabedoria, Destreza -1.</p>
            <p><strong>PV Iniciais:</strong> +14.</p>
        </div>
        <div class="habilidades">
            <p><strong>Devagar e Sempre:</strong> Seu deslocamento é 6m (em vez de 9m). Porém, seu deslocamento não é
                reduzido por uso de armadura ou excesso de carga.</p>
            <p><strong>Filho da Rocha:</strong> Você recebe visão no escuro em alcance médio e +1 ponto de vida por
                nível.</p>
            <p><strong>> Escolha uma das tradições abaixo:</strong></p>
            <p class="opcao">Tradição Artesã: Você recebe +2 em Ofício e, se for treinado neste ofício, pode fabricar
                itens superiores com uma melhoria.</p>
            <p class="opcao">Tradição das Minas: Você trata todos os machados, martelos, marretas e picaretas como armas
                simples e recebe +2 em ataques com essas armas.</p>
            <p class="opcao">Tradição da Pólvora: Você recebe proficiência com armas de fogo e +2 nas rolagens de ataque
                com essas armas.</p>
        </div>
    </div>

    <div class="raca">
        <h2>ELFO</h2>
        <div class="atributos">
            <p><strong>Atributos:</strong> +1 em um atributo mental, Destreza +1.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em um atributo mental, Des +1, Con -1.
            </p>
            <p><strong>PV Iniciais:</strong> +6.</p>
        </div>
        <div class="habilidades">
            <p><strong>Sangue Élfico:</strong> Você recebe +1 ponto de mana por nível e pode usar Sabedoria ou Carisma
                como atributo-chave de Misticismo (em vez de Inteligência).</p>
            <p><strong>Graciosidade Élfica:</strong> Seu deslocamento é 12m (em vez de 9m).</p>
            <p><strong>Sentidos Élficos:</strong> Você recebe visão no escuro em alcance curto e +2 em Percepção e
                Misticismo.</p>
            <p><em>Devido sua ligação com a magia, elfos têm acesso aos poderes raciais extraplanares.</em></p>
        </div>
    </div>

    <div class="raca">
        <h2>EXTRAPLANAR (fada/anjo/demônio)</h2>
        <div class="atributos">
            <p>Escolha um tamanho entre pequeno, médio ou grande. Uma vez feita a escolha, ela não pode ser alterada.
            </p>
            <p><strong>Atributos:</strong> +1 em três atributos.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em um atributo, +1 em um segundo
                atributo, -1 em um terceiro atributo.</p>
            <p><strong>PV Iniciais:</strong> +10.</p>
        </div>
        <div class="habilidades">
            <p><strong>Herança Extraplanar:</strong> Escolha dois poderes raciais ferais ou extraplanares.</p>
        </div>
    </div>

    <div class="raca">
        <h2>FERAL</h2>
        <div class="atributos">
            <p>Escolha um tamanho entre pequeno, médio ou grande. Uma vez feita a escolha, ela não pode ser alterada.
            </p>
            <p><strong>Atributos:</strong> +1 em três atributos.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em um atributo, +1 em um segundo
                atributo, -1 em um terceiro atributo.</p>
            <p><strong>PV Iniciais:</strong> +10.</p>
        </div>
        <div class="habilidades">
            <p><strong>> Escolha dois poderes raciais ferais.</strong></p>
        </div>
    </div>

    <div class="raca">
        <h2>GIGANTE/OGRO</h2>
        <div class="atributos">
            <p><strong>Atributos:</strong> Força +2, Constituição +1.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> Força +3, Constituição +2. -1 em Destreza,
                Sabedoria, Inteligência e Carisma.</p>
            <p><strong>PV Iniciais:</strong> +18.</p>
        </div>
        <div class="habilidades">
            <p><strong>Grandão:</strong> Seu tamanho é Grande (T20, pg 106). Você pode usar armas normais ou aumentadas,
                mas só pode vestir armaduras especialmente feitas para seu tamanho.</p>
            <p><strong>Couro Duro:</strong> Você recebe redução de dano igual a sua Constituição, limitada por seu
                nível.</p>
        </div>
    </div>

    <div class="raca">
        <h2>GNOMO/HALVELING</h2>
        <div class="atributos">
            <p><strong>Atributos:</strong> Destreza +1, +1 em Inteligência ou Carisma, +1 em um terceiro atribruto.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em Destreza, Inteligência ou Carisma, +1
                em um segundo atributo, -1 em Força.</p>
            <p><strong>PV Iniciais:</strong> +6.</p>
        </div>
        <div class="habilidades">
            <p><strong>Pequenino:</strong> Seu tamanho é Pequeno (T20, pg 106), mas seu deslocamento é 9m. Você pode
                usar Destreza como atributo-chave de Atletismo (em vez de Força).</p>
            <p><strong>> Sorte ou Ciência. Escolha uma das habilidades abaixo:</strong></p>
            <p class="opcao">Engenhosidade: Quando faz um teste de perícia, você pode gastar 2 PM para somar sua
                Inteligência no teste. Você não pode usar esta habilidade em testes de ataque.</p>
            <p class="opcao">Sorte Salvadora: Quando faz um teste de resistência, você pode gastar 1 PM para rolar este
                teste novamente.</p>
        </div>
    </div>

    <div class="raca">
        <h2>GOBLINOIDE</h2>
        <div class="atributos">
            <p>Escolha um tamanho entre pequeno (goblin, gremlin), médio (hobgoblin, orc) ou grande (bugbear, bakemono).
                Uma vez feita a escolha, ela não pode ser alterada.</p>
            <p><strong>Atributos:</strong> +1 em três atributos.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em Constituição, +1 em Força ou Destreza,
                -1 em Inteligência ou Carisma.</p>
            <p><strong>PV Iniciais:</strong> +10.</p>
        </div>
        <div class="habilidades">
            <p><strong>Natureza Bestial:</strong> Você recebe visão no escuro em alcance médio e pode usar Constituição
                em Intimidação (em vez de Carisma).</p>
            <p><strong>> Função na Horda. Escolha uma das funções abaixo:</strong></p>
            <p class="opcao">Bicho Papão: Enquanto estiver em alcance curto de uma criatura abalada ou apavorada, você
                recebe um bônus em testes de ataque e rolagens de dano igual à penalidade causada pela condição.</p>
            <p class="opcao">Combatente: Você recebe um poder de combate à sua escolha.</p>
            <p class="opcao">Engenhoso: Você não sofre penalidades em testes de perícia por não usar ferramentas. Se
                usar a ferramenta necessária, recebe +2 no teste de perícia.</p>
            <p class="opcao">Feroz: Você recebe +2 em rolagens de dano com armas corpo a corpo e de arremesso. Quando
                sofre dano de um inimigo, esse bônus se torna +4 até o fim de seu próximo turno.</p>
        </div>
    </div>

    <div class="raca">
        <h2>GOLEM</h2>
        <div class="atributos">
            <p>Escolha uma raça (exceto Extraplanar ou Morto-Vivo) para ser o seu modelo. Você possui todas as
                características da raça escolhida, mais as características Criatura Artificial e Fonte de Energia.</p>
        </div>
        <div class="habilidades">
            <p><strong>Criatura Artificial:</strong> Você é uma criatura do tipo construto. Recebe visão no escuro em
                alcance longo e imunidade a efeitos de cansaço, metabólicos e de veneno. Além disso, não precisa
                respirar, alimentar-se ou dormir, mas não se beneficia de cura mundana e de itens da categoria
                alimentação. Você precisa ficar inerte por oito horas por dia para recarregar sua fonte de energia. Se
                fizer isso, recupera PV e PM por descanso em condições normais (golens não são afetados por condições
                boas ou ruins de descanso). Por fim, a perícia Cura não funciona em você, mas Ofício (artesão) pode ser
                usada no lugar dela.</p>

            <p><strong>Fonte de energia. Escolha sua fonte de energia da lista abaixo:</strong></p>
            <p class="opcao">• Alquímica: Uma mistura alquímica gera a energia necessária à sua vida. Você pode gastar
                uma ação padrão para ingerir um item alquímico qualquer; se fizer isso, recupera 1 PM.</p>
            <p class="opcao">• Elemental: Você possui um espírito elemental preso em seu corpo. Escolha entre água
                (frio), ar (eletricidade), fogo (fogo) e terra (ácido). Você é imune a dano desse tipo. Se fosse sofrer
                dano mágico deste tipo, em vez disso cura PV em quantidade igual à metade do dano.</p>
            <p class="opcao">• Sagrada: Você foi animado por um texto ou símbolo sagrado depositado em seu corpo. Você
                pode lançar uma magia divina de 1º círculo à sua escolha (atributo-chave Sabedoria). Caso aprenda
                novamente essa magia, seu custo diminui em –1 PM.</p>
            <p class="opcao">• Vapor: Seu corpo é movido por vapor e engrenagens. Você é imune a dano de fogo; se fosse
                sofrer dano desse tipo, em vez disso seu deslocamento aumenta em 4,5m por 1 rodada. Entretanto, dano de
                frio deixa-o lento por 1 rodada.</p>
        </div>
    </div>

    <div class="raca">
        <h2>MORTO-VIVO</h2>
        <div class="atributos">
            <p>Escolha uma raça (exceto Extraplanar ou Golem). Era sua raça quando você era vivo. Você possui todas as
                características da raça escolhida, mais as características Natureza Morta-Viva e Preço da Não Vida.
                Escolha também o tipo de morto-vivo que você é: esqueleto, zumbi, aparição ou cria vampírica. Você
                possui acesso aos poderes raciais de morto-vivo de acordo com o tipo de morto-vivo que você escolheu.
            </p>
        </div>
        <div class="habilidades">
            <p><strong>Natureza Morta-Viva:</strong> Você é uma criatura do tipo morto-vivo. Recebe visão no escuro em
                alcance longo e imunidade a efeitos de cansaço, metabólicos, de trevas e de veneno. Além disso, não
                precisa respirar, alimentar-se ou dormir. Por fim, efeitos mágicos de cura de luz causam dano a você e
                você não se beneficia de itens da categoria alimentação, mas dano de trevas recupera seus PV.</p>

            <p><strong>Preço da Não Vida:</strong> Você precisa passar oito horas sob a luz de estrelas ou no
                subterrâneo. Se fizer isso, recupera PV e PM por descanso em condições normais (mortos-vivos não são
                afetados por condições boas ou ruins de descanso). Caso contrário, sofre os efeitos de fome.</p>
        </div>
    </div>

    <div class="raca">
        <h2>TROLL</h2>
        <div class="atributos">
            <p>Escolha um tamanho entre pequeno, médio ou grande. Uma vez feita a escolha, ela não pode ser alterada.
                Trows são trolls inteligentes e de tamanho médio.</p>
            <p><strong>Atributos:</strong> +1 em três atributos.</p>
            <p class="alternativo"><strong>Atributos Alternativos:</strong> +2 em Força ou Inteligência, +1 em
                Constituição, -1 em Inteligência ou Força.</p>
            <p><strong>PV Iniciais:</strong> +14.</p>
        </div>
        <div class="habilidades">
            <p><strong>Natureza Bestial:</strong> Você recebe visão no escuro em alcance médio e pode usar Constituição
                em Intimidação (em vez de Carisma).</p>
            <p><strong>Regeneração:</strong> Uma vez por rodada, você pode gastar 1 PM para recuperar 5 PV. Esta
                habilidade não cura dano de ácido ou fogo.</p>
        </div>
    </div>
</body>

</html>