# ⚔️ ENCOUNTER & COMBAT SYSTEMS

**[LOAD PRIORITY: ON-DEMAND — Load when designing combat encounters or resolving battles]**

---

## The Battlefield Action Design Rule (v2.5)

Every combat must include **narrative battlefield decisions**, not just attack rolls.

**Core Principle**: Combat is a scene, not just a math problem.

### Two-Phase Combat Structure

**Phase 1: THE TELL (Narrative Setup)**
- Describe battlefield environment
- Establish tactical elements (cover, hazards, objectives)
- Give NPCs personality through combat dialogue
- Create narrative choices beyond "I attack"

**Phase 2: THE RESOLUTION (Mechanical Execution)**
- Roll attacks, damage, saves
- Resolve narrative choices mechanically
- Track HP, conditions, resources
- Determine outcome

Tag: `[BATTLEFIELD ACTION: environment includes tactical elements, hazards, objectives beyond "kill everyone"]`

---

## Environmental Battlefield Elements

Every combat should have **interactive terrain**:

### The Five Battlefield Element Types

| Element | Description | Examples |
|---------|-------------|----------|
| **Cover** | Protection that blocks attacks | Pillars, walls, crates, trees |
| **Hazard** | Damage or danger zone | Fire, pit, acid, falling rocks |
| **Elevation** | High ground advantage | Cliffs, balconies, rooftops |
| **Mobility** | Movement challenges/advantages | Ropes, ladders, slippery ice, water |
| **Objective** | Goal beyond "kill enemies" | Rescue hostage, stop ritual, close portal |

**Baseline**: Every combat should include **at least 2** of these elements.

**Examples**:
- **Simple**: Cover (pillars) + Hazard (fire spreading)
- **Complex**: Cover (barricades) + Elevation (archer tower) + Objective (stop ritual)

Tag: `[COMBAT ENVIRONMENT: includes cover (pillars), hazard (spreading fire), objective (rescue hostage)]`

---

## Combat Objectives

Not every fight is "kill everything":

### Objective Types

**Victory Objectives** (how to win):
- **Eliminate**: Kill all enemies (standard)
- **Survive**: Last X rounds
- **Escape**: Get to exit point
- **Capture**: Subdue target alive
- **Protect**: Keep NPC/object safe
- **Stop**: Prevent ritual/action completion

**Bonus Objectives** (optional goals):
- No civilian casualties
- Minimal property damage
- Capture leader alive
- Recover stolen item

**Failure States** (lose conditions):
- Party wipes (standard)
- Protected NPC dies
- Ritual completes
- Enemy escapes with McGuffin

**Example**:
```
**Combat Objectives:**
- Victory: Stop ritual before completion (6 rounds)
- Bonus: Capture cult leader alive
- Failure: Ritual completes, demon summoned

Tag: [COMBAT OBJECTIVE: stop ritual within 6 rounds, bonus capture leader alive]
```

---

## Tactical NPC Behavior

NPCs should fight **intelligently, not suicidally**:

### Intelligence-Based Tactics

**Low Intelligence** (Animals, Undead, Oozes):
- Attack nearest target
- Simple patterns
- Fight to death unless trained

**Medium Intelligence** (Most Humanoids):
- Use cover and tactics
- Focus fire on wounded
- Retreat if outnumbered/outmatched
- Call for help

**High Intelligence** (Masterminds, Dragons):
- Exploit PC weaknesses
- Use environment strategically
- Have contingency plans
- Escape if losing

**Example**:
```
**Bandit Tactics (Medium Intelligence)**:
- Archers take cover behind crates
- Melee fighters focus on isolated PC
- Leader shouts orders, boosts morale
- If leader falls, bandits flee or surrender

Tag: [NPC TACTICS: bandits use cover, focus fire, flee if leader falls]
```

---

## Boss Encounter Design

Major villains get enhanced combat:

### Boss Features

**Hit Points**:
- Standard: Use stat block HP
- Boss: Add 50-100% HP for longer fight
- Epic Boss: Multiple HP pools ("phases")

**Action Economy**:
- Standard: One turn per round
- Boss: Legendary Actions (3 per round between PC turns)
- Epic Boss: Lair Actions (every initiative count 20)

**Phases**:
- Phase 1: Full health, basic tactics
- Phase 2: 50% HP, more dangerous abilities
- Phase 3: 25% HP, desperate/powerful moves

**Environmental Integration**:
- Boss uses lair features
- Summons minions mid-fight
- Triggers environmental hazards

**Example**:
```
**Vampire Lord Boss Fight**:
- HP: 250 (doubled from standard)
- Legendary Actions: 3/round (bite, move, charm)
- Lair Actions: Summon swarm of bats (initiative 20)
- Phases:
  - Phase 1 (100-75% HP): Confident, toys with PCs
  - Phase 2 (75-25% HP): Serious, uses legendary resistances
  - Phase 3 (<25% HP): Desperate, transforms to mist and tries to escape

Tag: [BOSS DESIGN: Vampire Lord, 250 HP, 3 legendary actions, 3 phases]
```

---

## Minion System

Low-HP enemies that die in one hit:

**Purpose**: Make PCs feel powerful without dragging out combat

**Rules**:
- 1 HP (any damage kills)
- Normal attack bonus and damage
- Come in groups of 4-8
- Used with boss fights or swarm encounters

**Example**:
- Boss fight includes 6 skeleton minions
- PCs can cut through minions easily
- Keeps action economy balanced (boss + minions vs. party)

Tag: `[MINIONS: 6 skeleton minions, 1 HP each, swarm the boss]`

---

## Combat Pacing

How long should combat last?

### Combat Duration Guidelines

| Duration | Rounds | Real Time | When to Use |
|----------|--------|-----------|-------------|
| **Quick** | 2-3 rounds | 10-15 min | Random encounter, weak enemies |
| **Standard** | 4-6 rounds | 20-30 min | Typical combat |
| **Boss** | 6-10 rounds | 40-60 min | Major villain, climactic battle |
| **Epic** | 10+ rounds | 60+ min | Campaign finale |

**Pacing Rule**: If combat drags past expected duration, escalate:
- Reinforcements arrive (for enemies or PCs)
- Environmental hazard activates
- Objective shifts (enemies try to escape)

Tag: `[COMBAT PACING: standard encounter, expect 4-6 rounds, 20-30 minutes]`

---

## Dynamic Combat Events

Keep combat interesting with mid-fight changes:

**Reinforcements**:
- Round 3: More enemies arrive
- Round 4: Ally NPC shows up to help

**Environmental Changes**:
- Round 2: Fire spreads, new hazard zones
- Round 4: Building collapses, new terrain

**Objective Shifts**:
- Round 3: Villain grabs hostage, tries to escape
- Round 5: Ritual reaches critical point, must be stopped NOW

**Morale Breaks**:
- Half enemies dead: Survivors flee or surrender
- Leader dies: Enemies scatter

Tag: `[DYNAMIC EVENT: Round 3 — fire spreads, creates new hazard zones]`

---

## Damage Narration

Make damage feel impactful:

### Damage Description Tiers

**Light Damage** (<25% max HP):
- "The blade grazes your shoulder"
- "You feel the impact but shake it off"

**Moderate Damage** (25-50% max HP):
- "The axe bites deep into your side"
- "You stagger from the blow, pain flaring"

**Heavy Damage** (50-75% max HP):
- "The strike nearly fells you, blood pouring"
- "You barely stay standing, vision blurring"

**Critical Damage** (75%+ max HP):
- "You collapse, fighting to stay conscious"
- "Everything goes red, you're on the edge"

**Killing Blow**:
- PC: "You feel life slipping away..." (start death saves)
- Enemy: "Your blade pierces their heart, they collapse lifeless"

Tag: `[DAMAGE NARRATION: describe based on HP percentage remaining]`

---

## Critical Hit Enhancement

Make crits memorable:

**Standard Crit**: Double damage dice
**Enhanced Crit**: Double damage + narrative effect

**Narrative Effects**:
- Knock enemy prone
- Disarm weapon
- Scar/maim (cosmetic)
- Sever limb (if lethal damage)
- Intimidate others (fear effect)

**Player Choice**: Let player describe their critical hit
- "How do you want to do this?" (when killing)
- Describe the flourish, the style, the impact

Tag: `[CRITICAL HIT: double damage + player describes killing blow]`

---

## Combat and Moral Consequence

Combat has moral weight (see [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md)):

**Tracking Kills**:
- Who did PC kill?
- Were they combatants or innocents?
- Self-defense or murder?

**Non-Lethal Options**:
- Knock enemies unconscious (declare before attack)
- Capture instead of kill
- Let enemies surrender

**Consequences**:
- Kill innocent: Major weight, haunts PC
- Kill in battle: Minor weight, add to register
- Spare enemy: Positive entry, may create ally

Tag: `[COMBAT MORALITY: track kills in Moral Consequence Register, offer surrender options]`

---

## Enemy Morale and Surrender

Not all enemies fight to death:

### Morale Break Conditions

**Surrender When**:
- Outnumbered 3:1 or more
- Leader killed or captured
- Lost 75% of forces
- Clear they cannot win

**Flee When**:
- Lost 50% of forces (if not fanatical)
- Objective secured (got what they came for)
- Outmatched (face overwhelming power)

**Fight to Death**:
- Fanatics (religious, cultists)
- Undead and constructs (no morale)
- Cornered with no escape
- Protect something more important than life

**Surrender Mechanics**:
- Enemy drops weapon, raises hands
- PCs choose: Accept, refuse, kill anyway
- Accepted surrender: Prisoners, interrogation, moral choice

Tag: `[ENEMY MORALE: bandits surrender if leader killed or 75% casualties]`

---

## Non-Combat Resolution

Sometimes combat can be avoided:

**Intimidation**: Scare enemies into fleeing or surrendering
**Persuasion**: Talk enemies down, negotiate
**Deception**: Trick enemies, avoid fight
**Stealth**: Avoid detection entirely

**When to Allow**:
- Enemies have motivation beyond "kill PCs"
- PCs have leverage (power, information, offer)
- Enemies are intelligent enough to reason

**When to Deny**:
- Enemies mindless or fanatical
- Orders are absolute ("kill on sight")
- PCs have nothing to offer

Tag: `[NON-COMBAT OPTION: enemies might surrender if intimidated, have self-preservation instinct]`

---

## Combat and Information Systems

Combat reveals information:

**Enemy Capabilities**:
- What attacks do they have?
- Special abilities, weaknesses
- Tactics and intelligence

**Enemy Goals**:
- What are they trying to do?
- Protect something? Retrieve something?
- Orders from higher up?

**World State**:
- Who are these enemies?
- Why are they here?
- What does this fight reveal about larger plot?

**Tag System**:
- `[COMBAT INFO: enemy tactics reveal military training — Information Tier: PUBLIC after fight]`

---

## Aftermath and Consequences

What happens after combat ends?

### Post-Combat Checklist

**Immediate**:
- Stabilize dying PCs/NPCs
- Short rest? Or press on?
- Loot and rewards

**Short-Term**:
- Prisoners (what to do with them?)
- Bodies (burial? burn? leave?)
- Alert others (fight was loud, reinforcements coming?)

**Long-Term**:
- Add casualties to Moral Consequence Register
- Update faction relationships (killed faction members)
- Living Clock tick (faction responds to losses)
- World state change (power vacuum, vengeance sworn)

Tag: `[COMBAT AFTERMATH: 3 prisoners taken, bodies alert nearby patrol in 10 minutes, faction vows vengeance]`

---

## Encounter Building Guidelines

How to design balanced combat:

### Encounter Difficulty (by APL)

**Easy**: 70% of party resources
**Medium**: 90% of party resources
**Hard**: 110% of party resources
**Deadly**: 130%+ of party resources

**Resources**: HP, spell slots, abilities, action economy

### Party Level Guidelines

**Levels 1-4** (Fragile):
- 3-4 encounters per day
- Deadly encounters can TPK
- Single enemy can down PC in one hit

**Levels 5-10** (Capable):
- 4-6 encounters per day
- PCs have more tools
- Can handle moderate challenge easily

**Levels 11-16** (Powerful):
- 5-7 encounters per day
- Hard to challenge
- Need multiple strong enemies or boss

**Levels 17-20** (Epic)**:
- 6-8 encounters per day
- Legendary creatures
- World-ending threats

Tag: `[ENCOUNTER BALANCE: party level 7, medium difficulty, 4 enemies of CR 4]`

---

## Combat Variety

Don't make every fight the same:

**Vary Objectives**: Not just "kill enemies"
**Vary Environment**: Different terrain each time
**Vary Enemies**: Different tactics, abilities
**Vary Scale**: Small skirmish vs. large battle

**Combat Types**:
- **Skirmish**: Standard fight
- **Chase**: Moving combat
- **Siege**: Defend or assault position
- **Duel**: 1v1 combat
- **War**: Massive battle (PCs are part of army)

Tag: `[COMBAT TYPE: chase scene, enemies pursuing PCs through city streets]`

---

## Common Combat Mistakes

❌ **Empty room fights** — Combat in featureless space
✅ **Interesting terrain** — Cover, hazards, elevation

❌ **Enemies fight stupidly** — Stand still and attack
✅ **Smart tactics** — Use environment, focus fire, retreat when losing

❌ **Every fight to the death** — No surrender or retreat
✅ **Morale matters** — Enemies flee or surrender when appropriate

❌ **Combat drags** — 2-hour slog through HP bags
✅ **Dynamic and paced** — Events, objectives, interesting choices

❌ **No narrative** — Just roll dice, no description
✅ **Tell the story** — Describe actions, damage, environment dramatically

---

## Combat Agency Rule (Live Sessions)

When running combat in **Live Session** mode ([52-LIVE-SESSION-MANAGEMENT.md](52-LIVE-SESSION-MANAGEMENT.md)), combat decisions are **exclusively** the domain of DMs and PCs.

### The Architect's Combat Role (Live)

**DO:**
- Narrate the battlefield environment and sensory details
- Present enemy intended actions for DM approval
- Suggest 3-5 possible actions per PC turn (with mechanical summaries)
- Track initiative order, HP, conditions, and Battlefield Action states
- Audit rule applications and remind of forgotten abilities
- Narrate results after DM/PC declares action and resolves rolls

**DO NOT:**
- ❌ Roll dice for anyone
- ❌ Choose PC or NPC actions without DM approval
- ❌ Override DM rulings
- ❌ Skip or rush player turns
- ❌ Decide combat outcomes unilaterally
- ❌ Fudge HP or stats without explicit DM approval

> *Combat is a collaborative scene. The Architect sets the stage and suggests choreography — the DM and PCs perform it.*

Tag: `[COMBAT AGENCY: DM and PCs decide — Architect audits and suggests]`

---

**See also:**
- [23-CREATURE-GENERATION.md](23-CREATURE-GENERATION.md) — Enemy design and resolution paths
- [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) — Combat and moral consequences
- [43-EMOTIONAL-SYSTEMS.md](43-EMOTIONAL-SYSTEMS.md) — Combat as emotional beat
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Post-combat ripple effects
- [52-LIVE-SESSION-MANAGEMENT.md](52-LIVE-SESSION-MANAGEMENT.md) — Live session combat facilitation
