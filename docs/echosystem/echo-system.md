
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ECHO SYSTEM RPG</title>
    <style>
        /* Reset and Base Styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f5f5f5;
            width: 100%;
            overflow-x: hidden;
        }

        /* Cover Styles */
        .cover-page {
            width: 100%;
            min-height: 100vh;
            padding: 2rem;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .cover-container {
            max-width: 800px;
            width: 90%;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }
        
        .title {
            font-size: clamp(2.5rem, 8vw, 4rem);
            font-weight: bold;
            color: #3498db;
            text-shadow: 3px 3px 0 #1a5276;
            letter-spacing: 3px;
            margin-bottom: 1rem;
        }
        
        .subtitle {
            font-size: clamp(1.5rem, 5vw, 2rem);
            color: #ecf0f1;
            text-shadow: 2px 2px 0 #7f8c8d;
            letter-spacing: 2px;
            margin-bottom: 2rem;
        }
        
        .author, .based-on {
            font-size: clamp(1rem, 3vw, 1.3rem);
            color: #bdc3c7;
            margin-top: 1rem;
        }
        
        .based-on {
            font-style: italic;
            color: #95a5a6;
        }

        
        .dice-decoration {
            position: absolute;
            opacity: 0.1;
            font-size: clamp(5rem, 15vw, 10rem);
            z-index: 1;
        }        
        .d20 {
            top: 20%;
            left: 10%;
            transform: rotate(15deg);
        }
        
        .d6 {
            bottom: 15%;
            right: 10%;
            transform: rotate(-20deg);
        }

        /* Main Content Styles */
        .main-content {
            width: 100%;
            max-width: 1000px;
            margin: 0 auto;
            padding: 2rem;
            background-color: white;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
        }

        /* Content Styling */
        h1, h2, h3, h4 {
            color: #2c3e50;
            margin: 1.5rem 0 1rem;
        }
        
        h1 {
            font-size: 2rem;
            border-bottom: 2px solid #3498db;
            padding-bottom: 0.5rem;
        }
        
        h2 {
            font-size: 1.7rem;
            background-color: #ecf0f1;
            padding: 0.5rem;
            border-radius: 4px;
        }
        
        h3 {
            font-size: 1.4rem;
            color: #2980b9;
        }
        
        h4 {
            font-size: 1.2rem;
            color: #3498db;
        }
        
        p {
            margin-bottom: 1rem;
        }
        
        /* Rules Sections */
        .rules-section {
            background-color: #f8f9fa;
            padding: 1.5rem;
            border-radius: 6px;
            margin: 1.5rem 0;
            border-left: 4px solid #3498db;
        }
        
        /* Lists */
        ul, ol {
            margin: 1rem 0;
            padding-left: 2rem;
        }
        
        li {
            margin-bottom: 0.5rem;
        }
        
        /* Dice and Skills Grid */
        .dice-list, .skill-category, .abilities-grid, .attribute-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1rem;
            margin: 1.5rem 0;
        }
        
        /* Cards */
        .dice-item, .skill-card, .ability-card, .attribute-card {
            background-color: white;
            border: 1px solid #e0e0e0;
            border-radius: 6px;
            padding: 1rem;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }
        
        /* Tags */
        .tag-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin: 1rem 0;
        }
        
        
        /* Responsive Adjustments */
        @media (max-width: 768px) {
            .main-content {
                padding: 1rem;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
        }
        
        .skills-table th{
            color: #1a5276;
            border: 1px solid #ddd;
        }
        .skills-table td {
            padding: 12px 15px;
            border: 1px solid #ddd;
        }
        
        .skills-table tbody tr {
            border-bottom: 1px solid #ddd;
        }
        
        .skills-table tbody tr:nth-of-type(even) {
            background-color: #f3f3f3;
        }
        
        .skills-table tbody tr:last-of-type {
            border-bottom: 2px solid #1a5276;
        }
        
        .primary-attr {
            font-weight: bold;
        }
        
        .secondary-attr {
            font-style: italic;
        }
        
        @media (max-width: 768px) {
            .skills-table {
                display: block;
                overflow-x: auto;
            }
        }
    </style>        
    </style>
</head>
<body>
    <!-- Cover Page -->
    <div class="cover-page">
        <div class="dice-decoration d6">⚀</div>
        <div class="dice-decoration d20">⚂	</div>
        <div class="cover-container">
            <h1 class="title">ECHO SYSTEM</h1>
            <h3 class="subtitle2">RPG</h3>
            <div class="author">Created by Ozy SSJ</div>
            <div class="based-on">Based on the NPSeeds Saga of Lia Keep</div>
        </div>
    </div>

    <!-- Main Content -->
    <div class="main-content">
        <!-- Your existing content here -->
        <h1>GENERAL RULES</h1>
        
        <h2>What is RPG?</h2>
        <p>RPG stands for <strong>Role-Playing Game</strong>, a form of gameplay where participants take on the roles of fictional characters and collaboratively create and experience a story in an imaginary world. Instead of simply watching or reading a narrative, players actively participate in it, describing their characters' actions, thoughts, and decisions. It's like improvised theater but with rules to define what can or cannot happen and dice to introduce an element of chance.</p>
        
        <p>In an RPG session, there is usually someone who acts as the narrator or <strong>Game Master (GM)</strong>, responsible for describing the setting, controlling non-player characters and creatures, and presenting challenges and situations to drive the story forward. The other participants are the players, who roleplay their own characters, each with distinct personalities, abilities, and goals. They react to what the GM presents and choose how to respond to obstacles, dialogues, or combat.</p>
        
        <p><strong>Dice</strong> come into play to determine whether actions succeed or fail. For example, if a character attempts to pick a locked door, the player might roll a die to see if they succeed. This rules system creates a balance between creative freedom and structure, allowing the story to unfold dynamically and unpredictably.</p>
        
        <p>In short, RPG is a collective experience of imagination and storytelling. It combines elements of gameplay with narrative and roleplaying, creating unique and memorable moments for everyone involved.</p>
        
        <h2>DICE AND ROLLS</h2>
        <p>You use a variety of multi-sided dice to determine different possible outcomes. Dice are named using the letter "d" followed by the number of faces they have. For example, a d100 is a hundred-faced die, and a d12 has twelve faces.</p>
        
        <p>The number before the die indicates how many dice to roll: <strong>2d8</strong> means you should roll two eight-sided dice.</p>
        
        <h2>CORE DICE</h2>
        <div class="dice-list">
            <div class="dice-item">
                <strong>D100</strong>: Used for checks. Roll 1d100 + bonuses against Difficulty % (DIF%)
            </div>
            <div class="dice-item">
                <strong>D4, D6, D8, D10, D12, D20</strong>: Used for damage, healing and other variable effects
            </div>
            <div class="dice-item">
                <strong>D2</strong>: Coin flip for yes/no decisions
            </div>
            <div class="dice-item">
                Some rolls use multipliers (e.g. 1d4 × 10)
            </div>
        </div>
        
        <h2>D100 ROLLS</h2>
        <p>Roll <strong>1d100 + bonuses</strong> vs <strong>DIF%</strong> to determine success</p>
        
        <div class="rules-section">
            <h3>Success:</h3>
            <ul>
                <li>Roll higher than DIF%</li>
                <li>Automatic success on natural 96-100</li>
            </ul>

            <h3>Failure:</h3>
            <ul>
                <li>Roll equal to or below DIF%</li>
                <li>Automatic failure on natural 1-5</li>
            </ul>
            
            <div class="note-box">
                <strong>Note:</strong> You must exceed DIF% to succeed. Matching counts as failure.
            </div>
        </div>
        
        <h3>Example Success:</h3>
        
        <div class="example">
            <p><strong>Ex1:</strong> Buccaneer Fayir wants to cross a narrow ramp to reach the roof of another building. This action requires an Acrobatics roll of DIF 80%. He has DEX 20 and Acrobatics II.</p>
            <p>He rolls <strong>1d100 + 20 + 2d20</strong> and gets <strong>89</strong>, a <span class="success">Success</span>.</p>
        </div>
        
        <div class="example">
            <p><strong>Ex2:</strong> Then, Fayir enters the vault room and tries to break it open. However, the vault has an arcane seal. Unlocking it is a very complex action. Require an Arcana test of DIF 130%. Fayir has INT 10 and Arcana I.</p>
            <p>He rolls <strong>1d100 + 10 + d20</strong> and gets <strong>64</strong> on the first roll and fails, but the buccaneer uses his special <span class="ability">Luck</span> ability to reroll one of dice of the failed test.</p>
            <p>On the second attempt, he gets <strong>112</strong>. It would be another failure, but Fayir rolled <strong>97</strong> on the d100 this time, which guarantees an <span class="success">automatic success</span>.</p>
        </div>

        <h3>Example Failure:</h3>
        
        <div class="example">
            <p><strong>Ex3:</strong> With the item from the safe in his possession, Fayir now needs to escape. The alarm goes off and he needs to lose the guards. Upon leaving the building, he gets into a carriage and begins his escape. He needs to perform a Piloting test of DIF 60% to escape. He has DEX 25 and Piloting III.</p>
            <p>The pirate rolls <strong>1d100 + 25 + 3d20</strong> and gets <strong>63</strong>. It would be enough to escape, but he rolled a <strong>3</strong> on the d100 - an <span class="failure">automatic failure</span>.</p>
        </div>        
        
        
        <h2>Attack Tests</h2>
        <div class="rules-section">
            <p>These are tests where the Difficulty (DIF) equals the target's defense. The main skills used in attack tests are:</p>
            <ul class="skill-list">
                <li><span class="skill">Fight</span></li>
                <li><span class="skill">Aim</span></li>
                <li><span class="skill">Spellcasting</span></li>
            </ul>
        </div>

        <h2>Resistance Tests</h2>
        <div class="rules-section">
            <p>These are tests where a target resists the DIF of a harmful effect. The main skills used in resistance tests are:</p>
            <ul class="skill-list">
                <li><span class="skill">Athletics</span></li>
                <li><span class="skill">Fortitude</span></li>
                <li><span class="skill">Perception</span></li>
                <li><span class="skill">Cognition</span></li>
                <li><span class="skill">Reflexes</span></li>
                <li><span class="skill">Presence</span></li>
            </ul>
        </div>

        <h2>ATTRIBUTES</h2>
        <div class="rules-section intro">
            <p>Attributes are numerical values representing a character's fundamental traits - physical strength, wit, agility, and personality. They form the basis for nearly all in-game actions and determine how skilled a character is in various areas.</p>
            <p>There are six primary attributes:</p>
        </div>

        <div class="attribute-grid">
            <div class="attribute-card">
                <h3 class="attribute-header">STRENGTH (STR)</h3>
                <p>Measures raw physical power, used for lifting weight, melee attacks, or forcing doors.</p>
                <div class="associated-skills">
                    <strong>Associated skills:</strong> Athletics and Fight.
                </div>
            </div>

            <div class="attribute-card">
                <h3 class="attribute-header">DEXTERITY (DEX)</h3>
                <p>Represents agility, reflexes, and coordination; it influences defense, stealth, ranged attacks, and light melee weapon attacks.</p>
                <div class="associated-skills">
                    <strong>Associated skills:</strong> Acrobatics, Riding, Stealth, Initiative, Sleight of Hand, Piloting, Aim, and Reflexes.
                </div>
            </div>

            <div class="attribute-card">
                <h3 class="attribute-header">CONSTITUTION (CON)</h3>
                <p>Shows physical endurance and health, affecting hit points and resistance to poison or disease.</p>
                <div class="associated-skills">
                    <strong>Associated skill:</strong> Fortitude.
                </div>
            </div>

            <div class="attribute-card">
                <h3 class="attribute-header">INTELLIGENCE (INT)</h3>
                <p>Evaluates logical reasoning, knowledge, and memorization ability.</p>
                <div class="associated-skills">
                    <strong>Associated skills:</strong> Alchemy, Arcana, Cognition, Spellcasting, Strategy, History, Investigation, Medicine, Nature, and Religion.
                </div>
            </div>

            <div class="attribute-card">
                <h3 class="attribute-header">SENSES (SEN)</h3>
                <p>Relates to perception, empathy, common sense, self-control, and intuition.</p>
                <div class="associated-skills">
                    <strong>Associated skills:</strong> Spellcasting, Insight, Initiative, Perception, and Survival.
                </div>
            </div>

            <div class="attribute-card">
                <h3 class="attribute-header">CHARISMA (CHA)</h3>
                <p>Reflects presence, personal magnetism, personality strength, and leadership or persuasion abilities.</p>
                <div class="associated-skills">
                    <strong>Associated skills:</strong> Animal Handling, Performance, Spellcasting, Deception, Intimidation, Persuasion, and Presence.
                </div>
            </div>
        </div>        
        
        
        <h2>ROLLING SKILLS</h2>
        <div class="rules-section intro">
            <p>Rolling Skills represent the specific abilities a character has mastered through training and experience. While attributes (Strength, Dexterity, Intelligence, etc.) reflect natural talents, skills show what a character can actually do with those talents.</p>
            <p>For example, a character might have high Strength but struggle to swim in a strong current without Athletics training. Another character with less natural strength but Athletics skill could navigate the water more effectively.</p>
            <p>Skill ranks range from I to IV, with each rank granting 1d20 to the attribute roll related to it.</p>
        </div>

    <h1>Rolling Skills Table</h1>
    
    <table class="skills-table">
        <thead>
            <tr>
                <th>Skill</th>
                <th>Primary Attribute</th>
                <th>Secondary Attribute</th>
                <th>Description</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Acrobatics</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">-</td>
                <td>
                <ul class="skill-uses">
                    <li>Balance checks</li>
                    <li>Standing up as bonus action (DIF 75%)</li>
                    <li>Squeezing through tight spaces</li>
                    <li>Moving through enemy space (vs target's Acrobatics, Initiative or Fight)</li>
                    <li>Escaping bonds (full action; vs Binder's Sleight of Hand, DIF 80% for nets, DIF 99% for manacles)</li>
                    <li>Riding</li>
                    <li>Can avoid grapples (vs grappler's Athletics DIF)</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Aim</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">Strength</td>
                <td>
                <ul class="skill-uses">
                    <li>Used for ranged attacks</li>
                    <li>Typically uses DEX, but thrown weapons can use STR</li>
                    <li>Some spells allow using Spellcasting attribute</li>
                    <li>No Aim bonus added for attacks with untrained weapons</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Animal Handling</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">Senses</td>
                <td>
                <ul class="skill-uses">
                    <li>Calm domestic animal (DIF 60%)</li>
                    <li>Command domestic animal (DIF 50%)</li>
                    <li>Calm wild animal (DIF 75%)</li>
                    <li>Command wild animal (DIF 60%)</li>
                    <li>Calm/command monsters (DIF 85%, only for INT -10 or lower monsters)</li>
                    <li>DIF increases by +10 if target is hostile</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Arcana</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">-</td>
                <td> 
                <ul class="skill-uses">
                    <li>Identify spells, magic items, or magical creatures (DIF 50 + creature level)</li>
                    <li>Operate arcane devices</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Athletics</td>
                <td class="primary-attr">Strength</td>
                <td class="secondary-attr">-</td>
                <td>
                <ul class="skill-uses">
                    <li>Running, climbing, swimming, jumping</li>
                    <li>Grappling</li>
                    <li>Can resist grapples (vs grappler's Athletics)</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Deception</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">Intelligence</td>
                <td>Lies and disguises</td>
            </tr>
            <tr>
                <td>Fight</td>
                <td class="primary-attr">Strength</td>
                <td class="secondary-attr">Dexterity</td>
                <td>
                <ul class="skill-uses">
                    <li>Used for melee attacks</li>
                    <li>Typically uses STR, but agile weapons can use DEX</li>
                    <li>Some spells allow using Spellcasting attribute instead</li>
                    <li>No Fight bonus added for attacks with untrained weapons</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Fortitude</td>
                <td class="primary-attr">Constitution</td>
                <td class="secondary-attr">-</td>
                <td>Physical resistance and vigor</td>
            </tr>
            <tr>
                <td>History</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">-</td>
                <td>Historical, political and geographical knowledge</td>
            </tr>
            <tr>
                <td>Intimidation</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">Strength</td>
                <td>Can roll Strength in physical situations</td>
            </tr>
            <tr>
                <td>Initiative</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">Senses</td>
                <td>Reaction time in combat</td>
            </tr>
            <tr>
                <td>Insight</td>
                <td class="primary-attr">Senses</td>
                <td class="secondary-attr">-</td>
                <td>Empathy, perception of intentions and motivations</td>
            </tr>
            <tr>
                <td>Investigation</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">-</td>
                <td>
                <ul class="skill-uses">
                    <li>Unlike Perception, Investigation requires active reasoning and cognition</li>
                    <li>Researching, gathering information</li>
                    <li>Some situations allow using CHA for Investigation when dealing with people</li>
                </ul>
                </td>
            </tr>          
            <tr>
                <td>Medicine</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">Senses</td>
                <td>Medical diagnosis and healing</td>
            </tr>
            <tr>
                <td>Nature</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">Senses</td>
                <td>Knowledge of the natural world</td>
            </tr>
            <tr>
                <td>Percepction</td>
                <td class="primary-attr">Senses</td>
                <td class="secondary-attr">-</td>
                <td>Observation of the environment and sensory qualities</td>
            </tr>
            <tr>
                <td>Performance</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">-</td>
                <td>Performing arts</td>
            </tr>
            <tr>
                <td>Persuasion</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">-</td>
                <td>Diplomacy and negotiation</td>
            </tr>
            <tr>
                <td>Presence</td>
                <td class="primary-attr">Charisma</td>
                <td class="secondary-attr">-</td>
                <td>Personality strength against the effects of control and manipulation</td>
            </tr>
            <tr>
                <td>Reasoning</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">-</td>
                <td>Logic and problem-solving and resistance against mental effects</td>
            </tr>
            <tr>
                <td>Reflexes</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">-</td>
                <td>Quick dodges and agile movements</td>
            </tr>
            <tr>
                <td>Religion</td>
                <td class="primary-attr">Intelligence</td>
                <td class="secondary-attr">Senses</td>
                <td>Divine, theological and ritualistic knowledge</td>
            </tr>
            <tr>
                <td>Sleight of Hand</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">Intelligence</td>
                <td>Steal, pick locks, disable traps</td>
            </tr>

            <tr>
                <td>Spellcasting</td>
                <td class="primary-attr">Charisma, Intelligence, Senses</td>
                <td class="secondary-attr">-</td>
                <td>
                <ul class="skill-uses">
                    <li>Used to cast spells</li>
                    <li>Make magical attacks</li>
                    <li>Determine spell resistance DCs (Passive Spellcasting)</li>
                    <li>Some abilities allow using physical attributes instead of mental ones for Spellcasting</li>
                </ul>
                </td>
            </tr>
            <tr>
                <td>Stealth</td>
                <td class="primary-attr">Dexterity</td>
                <td class="secondary-attr">-</td>
                <td>Silent movement and concealment</td>
            </tr>
            <tr>
                <td>Survival</td>
                <td class="primary-attr">Senses</td>
                <td class="secondary-attr">Intelligence</td>
                <td>Orientation and tracking in nature</td>
            </tr>
        </tbody>
    </table>

        <div class="rules-section formula">
            <h3>Passive Skill Value</h3>
            <p>The base value of a skill used as Difficulty Percentage (DIF) for abilities or Defense.</p>
            <div class="calculation-box">
                <strong>Calculated as:</strong> 50 + related attribute + skill rank x 10
            </div>
        </div>        
        
        <h2>OTHER FEATURES</h2>
        <div class="abilities-grid">

            <div class="ability-card">
                <h4 class="ability-name">Hit Points (HP)</h4>
                <div class="ability-description">
                    <p>Quantification of a character's health.</p>
                    <p>Formula: Constitution + (Level x HP per Class Level).</p>
                </div>

            </div>
            <div class="ability-card">
                <h4 class="ability-name">Mana Points (MP)</h4>
                <div class="ability-description">
                    <p>Quantification of a character's magic pool.</p>
                    <p>Formula: Main mental attribute + (Level x MP per Class Level).</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Defenses (DEF)</h4>
                <div class="ability-description">
                    <p> DIF% of skills used as defense against attacks and other harmful effects.</p>
                    <p>Formula: 50 + Atribute + skill rank x 10.</p>
                    <p><strong>Main Defenses:</strong></p>
                    <p><strong>RefDef:</strong> Reflex Defense. The main defense against physical attacks.</p>
                    <p><strong>PerDef:</strong> Perception Defense, used mainly against stealth rolls.</p>
                    <p><strong>WilDef:</strong> Will Defense, used mainly against Persuasion rolls and mind controll.</p>
                    <p><strong>ForDef:</strong> Fortitude Defense, used against physical stress.</p>
                    <p><strong>AthDef:</strong> Athletics Defense, used against brute force.</p>
                    <p><strong>CogDef:</strong> Cognition Defense, used against mental and intellectual stress.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Attacks (ATK)</h4>
                <div class="ability-description">
                    <p> DIF% of skills used for saving throws.</p>
                    <p>Formula: 50 + Atribute + Skill.</p>
                    <p><strong>Main Attacks:</strong></p>
                    <p><strong>Meelee Attack:</strong> Meelee Attack DIF%: 50 + STRENGH + Fight rank x 10.</p>
                    <p><strong>Ranged Attack:</strong> Ranged Attack DIF%: 50 + DEXTERITY + Aim  rank x 10.</p>
                    <p><strong>Magical Attack:</strong> Magical Attack DIF%: 50 + Spellcasting Attribute + Spellcasting rank x 10.</p>
                </div>
            </div>



        </div>

        <h2>OTHER SKILLS</h2>
        <div class="rules-section intro">
            <p>Feats are powers characters gain through their species and class as they level up.</p>
        </div>

        <div class="abilities-grid">
            <div class="ability-card">
                <h4 class="ability-name">Elemental Affinity I</h4>
                <div class="ability-description">
                    <p>Learn two 1st-tier spells from one of your elemental affinities.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Elemental Affinity II</h4>
                <div class="ability-description">
                    <p>Learn two 2nd-tier spells from one affinity or upgrade two known spells to 2nd-tier.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Light Blade Training</h4>
                <div class="ability-description">
                    <p>Use shortswords, rapiers, scimitars, and daggers in Fight tests.</p>
                    <p>May substitute Dexterity for Strength on attack rolls.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Heavy Blade Training</h4>
                <div class="ability-description">
                    <p>Use longswords, bastard swords, and greatswords in Fight tests.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Attribute Progression</h4>
                <div class="ability-description">
                    <p>+5 to one attribute.</p>
                    <p>Can only select this ability for the same attribute once every 25 levels.</p>
                </div>
            </div>

            <div class="ability-card">
                <h4 class="ability-name">Skill Progression</h4>
                <div class="ability-description">
                    <p>+5 to one skill.</p>
                    <p>Can only select this ability for the same skill once every 20 levels.</p>
                </div>
            </div>
        </div>
        
        <h2>CHARACTER CREATION</h2>
        <div class="rules-section intro">
            <p>To create a character, follow these steps:</p>
            <ol class="creation-steps">
                <li>Distribute attribute points</li>
                <li>Choose a species</li>
                <li>Choose a class</li>
                <li>Choose a role</li>
            </ol>
        </div>

        <h3>ATTRIBUTE DISTRIBUTION</h3>
        <div class="rules-section">
            <p>You receive <strong>35 points</strong> to allocate among your six attributes. You may reduce an attribute by up to <strong>-5</strong> to gain extra points. The maximum attribute value cannot exceed <strong>15</strong>.</p>
        </div>
        
        
    </div>
</body>
</html>
