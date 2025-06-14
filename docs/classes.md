<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <title>Classes - Auramana T20</title>
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


  .classe-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
    margin-top: 30px;
  }

  .classe-card {
    background-color: rgba(187, 168, 140, 0.1);
    border-left: 4px solid var(--cor-primaria);
    border-radius: 0 5px 5px 0;
    padding: 20px;
    transition: all 0.3s;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
  }

  .classe-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
  }

  .classe-header {
    display: flex;
    align-items: center;
    margin-bottom: 15px;
  }

  .classe-icon {
    width: 50px;
    height: 50px;
    margin-right: 15px;
    object-fit: contain;
  }

  h1, h2, h3 {
    color: var(--cor-primaria);
    text-shadow: 1px 1px var(--cor-destaque);
    border-bottom: 2px solid var(--cor-primaria);
    padding-bottom: 5px;
  }

  .btn {
    display: inline-block;
    background-color: var(--cor-primaria);
    color: #fff9e6;
    padding: 8px 16px;
    border-radius: 5px;
    margin-top: 10px;
    text-decoration: none;
    transition: all 0.3s;
  }

  .btn:hover {
    background-color: var(--cor-secundaria);
  }
</style>

# Classes de Auramana

As sete classes fundamentais que moldam os destinos de Auramana:

<div class="classe-grid">

  <!-- Arcanista -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Arcanista</h2>
    </div>
    <p>Mestres da magia erudita que dominam os segredos arcanos através de estudo e disciplina.</p>
    <p><strong>Atributo-Chave:</strong> Inteligência Carisma ou Sabedoria</p>
    <a href="classes/arcanista.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Batedor -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Batedor</h2>
    </div>
    <p>Especialistas em combate tático, movimentos precisos e ataques furtivos.</p>
    <p><strong>Atributo-Chave:</strong> Destreza</p>
    <a href="classes/batedor.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Elementalista -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Elementalista</h2>
    </div>
    <p>Manipuladores das forças primordiais da natureza e dos elementos.</p>
    <p><strong>Atributo-Chave:</strong> Sabedoria, Carisma ou Inteligência</p>
    <a href="classes/elementalista.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Guerreiro -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Guerreiro</h2>
    </div>
    <p>Combatentes versáteis e resilientes, mestres de todas as formas de armas.</p>
    <p><strong>Atributo-Chave:</strong> Força, Destreza ou Constituição</p>
    <a href="classes/guerreiro.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Inspirador -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Inspirador</h2>
    </div>
    <p>Líderes carismáticos que motivam aliados e influenciam situações.</p>
    <p><strong>Atributo-Chave:</strong> Carisma</p>
    <a href="classes/inspirador.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Inventor -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Inventor</h2>
    </div>
    <p>Criadores de engenhocas e dispositivos que desafiam as leis da natureza.</p>
    <p><strong>Atributo-Chave:</strong> Inteligência</p>
    <a href="classes/inventor.md" class="btn">Ver Detalhes</a>
  </div>

  <!-- Sacerdote -->
  <div class="classe-card">
    <div class="classe-header">
      <h2>Sacerdote</h2>
    </div>
    <p>Canalizadores do poder divino, seja para cura, proteção ou destruição.</p>
    <p><strong>Atributo-Chave:</strong> Sabedoria, Inteligência ou Carisma</p>
    <a href="classes/sacerdote.md" class="btn">Ver Detalhes</a>
  </div>

</div>

<div style="text-align: center; margin-top: 40px;">
  <a href="ficha.md" class="btn" style="padding: 12px 24px; font-size: 1.1em;">
    Criar Ficha de Personagem
  </a>
</div>