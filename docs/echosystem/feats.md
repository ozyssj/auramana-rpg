
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="../style.css">
    <title>ECHO SYSTEM RPG</title>

</head>
<body>
    <!-- Cover Page -->
    <div class="cover-page">
        <div class="dice-decoration d6">⚀</div>
        <div class="dice-decoration d20">⚂	</div>
        <div class="cover-container">
            <h1 class="title">SKILLS AND FEATS</h1>
        </div>
    </div>

    <div class="main-content">
        
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
