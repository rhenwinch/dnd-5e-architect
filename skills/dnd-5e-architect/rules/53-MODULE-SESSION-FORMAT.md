# 📖 PRE-PLANNED MODULE FORMAT

**[LOAD PRIORITY: CONDITIONAL — Load when DM chooses Pre-Planned Module mode for session delivery]**

---

## Purpose

When the DM chooses **Pre-Planned Module** mode, The Architect generates a **modular adventure** — a collection of standalone quest and situation modules the DM can run in any order based on player choices.

> **This is NOT a session-by-session script.** It is a toolkit of prepared situations, quests, locations, and encounters — like *Dragon of Icespire Peak* — where ALL possibilities are planned and written, and the DM selects what to run based on what the players choose to do.

Tag: `[QUEST MODULE: quest name — tier/level range]`

---

## The Players' Story Doctrine

> **What you prep might NOT be what the players will do. It is THEIR story, not yours.**

This is the single most important rule of module generation. Every module, every quest, every situation exists as a **possibility** — not a mandate. The players decide which situations to engage with, in what order, and by what approach.

### The Anti-Linear Mandate

1. **Modules are situations, not sessions.** A module describes WHAT IS HAPPENING in a location or with a faction — not what happens on a specific night of play. The DM runs whichever module fits what the players chose to do.
2. **No predetermined sequence.** Module A does not "lead to" Module B unless there is a justified prerequisite (see When Railroading is Justified). The party might do Module C first, skip Module A entirely, and invent Module F that you never wrote.
3. **Session numbers are DM bookkeeping, not module identity.** The DM might run the "Gnoll Warren" quest module on session 3, session 7, or never. It doesn't matter. The module is ready whenever the players go there.
4. **Prep the world, let the players write the story.** The campaign's driving force creates urgency. The Living Clock creates consequences. But the PLAYERS decide how they engage with both.

### What This Means in Practice

- **BAD:** Generating `session-01-module.md` → `session-02-module.md` → `session-03-module.md` with session 2 assuming session 1's outcomes
- **GOOD:** Generating `quest-tower-of-storms.md`, `quest-gnoll-warren.md`, `quest-merchants-plea.md` — any of which the party might pursue on any session night
- **BAD:** "After the party defeats the bandits, they learn about the missing caravan" (assumes sequence)
- **GOOD:** "The missing caravan is a known situation. The party can learn about it from multiple sources: the job board, tavern rumors, the merchant NPC, or encountering the wreckage during travel."

---

## When Railroading Is Justified

Railroading — directing players toward specific content — is PROHIBITED by default. However, there are narrow, mechanically justified exceptions where **soft gates** or **prerequisites** are appropriate:

### Justified Prerequisites

| Gate Type | When It's Justified | Example | How to Signal |
|---|---|---|---|
| **CR / Level Gate** | Encounter would be lethal for underleveled PCs | "The ancient dragon's lair is designed for level 10+ parties" | Mark in quest header: `**Recommended Level:** 10+`. Include a warning encounter or NPC that signals danger. |
| **Item / Key Requirement** | A specific object is needed to access a location | "The Vault of Whispers requires the Sunstone Key" | List the prerequisite in the quest header. Ensure the required item is obtainable from 2+ different quests. |
| **Knowledge Gate** | Players need specific information to understand a situation | "The ritual's meaning is unknown without translating the glyphs" | Make the knowledge discoverable through multiple paths (portable secrets). |
| **Story Prerequisite** | A prior event must logically have occurred | "The rebel faction only forms AFTER the king's decree" | Use Living Clock to trigger the situation at the right world-state. |
| **Safety Gate** | Content requires table consent (horror, sensitive themes) | "This quest involves body horror elements" | Flag in quest header with content warning. |

### Rules for Prerequisites

1. **Minimize them.** Most quests should have ZERO prerequisites. A player should be able to walk into most situations cold.
2. **Never single-source a prerequisite.** If quest B requires information from quest A, that same information MUST also be available from at least one other source (a different NPC, location, or faction path).
3. **Signal danger, don't block access.** For CR gates, don't lock the door — post warning signs. Let players flee. An NPC who says *"No one who enters the Ash Mines below level 8 comes back alive"* is a signal. A locked door that requires level 8 is a railroad.
4. **Mark prerequisites clearly.** Every quest module header lists prerequisites (if any) so the DM can see at a glance what's accessible.

Tag: `[PREREQUISITE: type — requirement — alternative paths: X]`
Tag: `[RAILROAD JUSTIFIED: reason — gate type]`

---

## The Module Standard

> **Every quest module must be indistinguishable in quality and structure from a professionally published D&D adventure module. If a DM handed this to a player, they should believe it came from Wizards of the Coast.**

### What This Means

- **Narrative prose** — not bullet-point outlines. Read-aloud text is written in evocative, atmospheric prose.
- **DM Notes** — inline guidance boxes that help the DM anticipate player actions and adapt.
- **Complete encounters** — with stat references, tactics, terrain, and scaling notes.
- **NPC dialogue** — key lines of dialogue and personality cues, not just "NPC talks to party."
- **Maps and area descriptions** — detailed room/area descriptions with sensory details (sight, sound, smell, temperature).
- **Rewards and consequences** — clearly stated outcomes for success, failure, and creative solutions.
- **Self-contained** — each module contains everything the DM needs. No consulting other files during play.
- **Order-independent** — modules work regardless of what the party has done before (unless a justified prerequisite exists).

---

## Module Architecture: The Quest Board Model

Campaign modules follow the **Quest Board Model** (inspired by *Dragon of Icespire Peak*). Instead of a linear chain of session-numbered files, The Architect generates:

### 1. Campaign Guide (`[campaign-name]-guide.md`)
The master document for the DM. Contains:
- Campaign overview, driving force, and premise
- **Quest Board** — a table of all available quest modules with names, level ranges, prerequisites, brief descriptions, and current status (available / locked / completed)
- Faction overview and Living Clock stages
- Regional map / location index
- PC hooks and connections
- Campaign-wide DM notes and contingencies

### 2. Quest Modules (`[campaign-name]-quest-[quest-name].md`)
Standalone adventure modules, each describing **one situation, quest, or location**. The DM pulls the relevant quest module when the players choose to engage with that content.

### 3. Session Log (`[campaign-name]-session-log.md`)
After each session, the DM (or Architect) records what actually happened — which modules were used, what players did, what consequences were generated. Session numbers live HERE, not in the modules themselves.

---

## Module File Naming

### Quest Modules
**File:** `[campaign-name]-quest-[quest-name].md`

**Location:** `worlds/[world-name]/campaigns/[campaign-name]/`

**Examples:**
- `shadow-crown-quest-tower-of-storms.md`
- `shadow-crown-quest-gnoll-warren.md`
- `shadow-crown-quest-merchants-plea.md`
- `shadow-crown-quest-the-sunken-temple.md`
- `broken-gods-quest-fallen-sanctum.md`

### Campaign Guide
**File:** `[campaign-name]-guide.md`

**Examples:**
- `shadow-crown-guide.md`
- `broken-gods-guide.md`

---

## Quest Module Template Structure

Every quest module MUST follow this structure. Sections marked with ★ are mandatory. Sections marked with ◆ are included when relevant.

```markdown
# [Campaign Name] — Quest: [Quest Title]

**Campaign:** [Campaign Name]
**Quest Type:** [Main Quest / Side Quest / Faction Quest / Exploration / Event]
**Recommended Level:** [X-Y] | **Tier:** [1-4]
**Estimated Duration:** [1-2 sessions / single session / half-session]
**DM Complexity:** [★☆☆☆☆ to ★★★★★] — [Brief justification]
**Prerequisites:** [None / List specific requirements with alternative paths]
**Location:** [Where this quest takes place]
**Themes:** [2-3 thematic keywords]
**Tone:** [Primary tone from eight-tone palette]
**Driving Force Connection:** [How this quest connects to the campaign's central tension]
**Status:** [Available / Locked (prerequisite) / Triggered (by Living Clock)]

---

## ★ Quest Overview

[2-3 paragraph overview of the situation. Written for the DM's eyes only.
Describes WHAT IS HAPPENING — the active situation, the forces involved,
and what's at stake. Does NOT assume when or in what order the party
arrives. Includes the quest's dramatic question.]

**The Situation:** [1-2 sentence summary of the active situation]
**Dramatic Question:** [The central question this quest answers]
**Discovery Hooks:** [How the party can learn about this quest — list 3+
sources: quest board, NPC rumor, faction request, travel encounter,
personal hook, world event, etc.]

> **💡 DM TIP:** [When to introduce this quest. What signals suggest
> the party is ready for it. How to seed it naturally.]

---

## ★ Quest Opening

### Read-Aloud Text: Arrival

> *[Atmospheric boxed text the DM reads when the party arrives at the
> quest location or first encounters the situation. Written in second
> person present tense. 3-5 sentences. Does NOT assume how or why
> the party is here.]*

### Scene Setup
- **Location:** [Where the PCs are]
- **Time:** [Flexible — adapt to when the party arrives]
- **Weather/Atmosphere:** [Environmental conditions]
- **Immediate Situation:** [What the PCs see/hear/feel right now]
- **What Has Changed:** [If the Living Clock has advanced, note what's
  different from the default state described above]

> **💡 DM TIP:** [How to adapt this opening based on the party's
> approach — did they come seeking this quest, stumble into it, or
> arrive from an unexpected direction?]

---

## ★ Situations and Scenes

[Quest modules contain SITUATIONS — active forces and events happening
in this location/quest. They are NOT ordered acts. The DM uses whichever
scenes are relevant based on what the players do.]

### Situation: [Situation Title]

[Narrative description of this situation — what is happening, who is
involved, and what the active forces are. 1-2 paragraphs. Describes
the CURRENT STATE, not a scripted sequence.]

#### Scene [X]: [Scene Title]

##### Read-Aloud Text

> *[Boxed text for this scene. Atmospheric, sensory-rich prose.]*

##### Scene Details
- **Purpose:** [Why this scene exists — what it advances]
- **Trigger:** [What causes this scene to occur — player arrival, NPC action,
  time passing, player choice, or always active]
- **Key NPCs Present:** [Names with brief reminder of who they are]
- **Key Information Available:** [What PCs can learn here]
- **Mood:** [The emotional tone of this scene]
- **Portable:** [Yes/No — can this scene be relocated if players go elsewhere?]
- **Suggested Ambiance:** [Music/sound cue]

##### NPC Roleplay Guide

**[NPC Name]** — [Race, role, 1-line personality]
- **Motivation:** [What they want RIGHT NOW]
- **Demeanor:** [How they act — nervous, commanding, secretive]
- **Key Dialogue:**
  - *"[Important line that reveals character or advances plot]"*
  - *"[Response to likely PC question]"*
  - *"[Fallback line if conversation stalls]"*
- **Secret:** [What they're hiding, if anything]
- **Portable:** [Can this NPC appear elsewhere if the party doesn't come here?]
- **Stat Reference:** [Book/page or custom stat block reference]

> **💡 DM TIP:** [How to play this NPC, what to do if PCs are
> suspicious, aggressive, or try to skip this interaction.]

##### Skill Challenges / Checks

| Check | DC | Success | Failure |
|---|---|---|---|
| [Skill] | [DC] | [What happens] | [What happens] |

##### Player Approaches

The party may approach this situation in multiple ways:
- If PCs choose [approach A]: → [What happens — reference Scene X if relevant]
- If PCs choose [approach B]: → [What happens — reference Scene Y if relevant]
- If PCs avoid this entirely: → [What happens in the world — Living Clock advances]
- If PCs do something unexpected: → See **DM Contingency** in Appendices

> **💡 DM TIP:** [The players' choices matter more than your prep.
> If they find a creative solution not listed here, reward it.
> Never funnel them back to your planned path.]

### ◆ Rest Opportunity

**Rest Type:** [Short Rest / Long Rest / None]
**Narrative Justification:** [Why a rest makes sense here — safe location,
time skip, NPC hospitality, etc.]
**If PCs Skip Rest:** [Consequence — resource depletion warning, fatigue
effects, or no penalty if rest is optional]

> **💡 DM TIP:** [Whether to encourage or discourage rest here based on
> pacing and upcoming encounter difficulty.]

---

## ◆ Exploration Areas

### ◆ Exploration Area: [Area Name]

#### Area Overview
[General description of the area — what it looks like, feels like,
and why it matters. This area exists in the world whether or not
the party visits it.]

#### Keyed Locations

**[Area Code]. [Room/Location Name]**

> *[Read-aloud text for this specific area. 2-4 sentences.]*

- **Dimensions:** [Size description]
- **Light:** [Bright, dim, darkness]
- **Features:** [Notable objects, furniture, terrain]
- **Creatures:** [What's here — stat reference]
- **Treasure:** [What can be found — with story connection]
- **Traps/Hazards:** [If any — DC, damage, effect]
- **Connections:** [Doors/passages to other areas]
- **Secret:** [Hidden elements — Perception/Investigation DC to find]

> **💡 DM TIP:** [What to emphasize, what to skip if pressed for time,
> how this area connects to the larger story.]

### ◆ Encounter: [Encounter Title]

#### Encounter Overview
- **Type:** [Combat / Social / Exploration / Mixed]
- **Difficulty:** [Easy / Medium / Hard / Deadly]
- **Estimated Duration:** [15 / 30 / 45 / 60 minutes]
- **Connection Test:** [How this encounter connects to the campaign — plot/faction/character/theme/consequence]

#### Tactical Setup
- **Terrain:** [Description of the battlefield/environment]
- **Environmental Features:** [Cover, elevation, hazards, interactive elements]
- **Lighting:** [Bright light, dim light, darkness zones]
- **Starting Positions:** [Where enemies are, where PCs enter]

#### Enemy Forces

| Creature | Count | HP | AC | Key Abilities | Tactics |
|---|---|---|---|---|---|
| [Name] | [#] | [HP] | [AC] | [1-2 key abilities] | [Brief tactical behavior] |

**Stat References:** [Book/page for full stat blocks, or include custom stat block below]

#### Enemy Tactics
- **Round 1:** [What enemies do first]
- **Round 2-3:** [How tactics evolve]
- **Low HP / Morale:** [When they flee, surrender, or fight harder]
- **Boss Behavior:** [If applicable — legendary actions, lair actions, phases]

#### Scaling Notes
- **Fewer PCs / Lower Level:** [How to make easier]
- **More PCs / Higher Level:** [How to make harder]
- **PCs Struggling:** [Emergency escape valve or DM intervention]

#### Read-Aloud: Combat Start

> *[Atmospheric text for when initiative is rolled. Sets the scene
> for combat. 2-3 sentences.]*

#### Read-Aloud: Combat End

> *[Atmospheric text for when combat concludes. Describes the
> aftermath. Varies by outcome — victory, retreat, or loss.]*

> **💡 DM TIP:** [Common player strategies and how enemies respond.
> What makes this fight memorable vs. just another combat.]

### ◆ Rest Opportunity

**Rest Type:** [Short Rest / Long Rest / None]
**Narrative Justification:** [Why a rest makes sense here — safe room
cleared, allies provide shelter, time skip, etc.]
**If PCs Skip Rest:** [Consequence — upcoming climax difficulty warning
or mechanical penalty]

> **💡 DM TIP:** [Pacing consideration — is a rest here desirable for
> the climax difficulty, or should pressure be maintained?]

---

## ★ Quest Climax

[Description of the dramatic high point of this quest — what makes
this moment matter, what's at stake. This is the natural culmination
of the situation, NOT a scripted Act 3. It triggers when the players
have engaged with the situation deeply enough.]

### Trigger Conditions
[What circumstances bring the quest to its climax — player actions,
time passing, faction moves, or NPC escalation]

#### Possible Outcomes
- **Victory/Success:** [What happens if PCs succeed — narrative and mechanical]
- **Partial Success:** [What happens if PCs partially succeed]
- **Failure:** [What happens if PCs fail — consequences, not game-over]
- **Creative Solution:** [Reward for unexpected clever solutions]
- **Abandoned / Ignored:** [What happens in the world if the party
  never engages with this quest — Living Clock consequences]

> **💡 DM TIP:** [How to make the climax feel earned. What emotional
> beats to hit. Remember: this might happen in session 2 or session
> 12 — it doesn't matter. The payoff comes from the situation, not
> the calendar.]

---

## ★ Quest Resolution and Consequences

### Outcomes
[What happens after the climax. How the world changes based on
the result. 1-2 paragraphs per major outcome path.]

### Consequences Generated
| Decision/Event | Immediate Consequence | Future Consequence | Affects Which Quests |
|---|---|---|---|
| [What happened] | [What changes now] | [What will matter later] | [Other quest modules affected] |

### Connections to Other Quests
[How this quest's completion (or failure) affects the availability,
difficulty, or nature of other quest modules in the campaign.
List specific cross-references.]

### Rewards
| Item | Type | Value | Story Connection | How Earned |
|---|---|---|---|---|
| [Name] | [Type] | [GP value] | [Why it matters] | [Which outcome] |

**Experience / Milestones:**
- [XP awards or milestone progression for this quest]

> **💡 DM TIP:** [What threads this resolution opens. What new
> situations emerge from the outcome. How to hook the party into
> their next chosen quest.]

---

## ★ Appendices

### Appendix A: NPC Quick Reference

| NPC | Race/Class | Role | Location | Key Trait | Secret |
|---|---|---|---|---|---|
| [Name] | [Info] | [Role] | [Where] | [1-word trait] | [Hidden info] |

### Appendix B: Stat Blocks

[Full stat blocks for any custom creatures or modified NPCs used
in this quest. Use standard D&D 5e stat block format.]

### ◆ Appendix C: Handouts and Player Information

[Any handouts, letters, maps, or documents the PCs might find.
Formatted as in-world documents the DM can show/read to players.
Each handout follows the Handout Generation Standard below.]

**Handout [Number]: [Handout Title]**
- **Type:** [Letter / Journal Entry / Contract / Wanted Poster / Map Fragment / Inscription / Notice / Other]
- **Found At:** [Scene/location where PCs discover this]
- **Condition:** [Pristine / Aged / Torn / Water-damaged / Partially burned / Blood-stained]
- **Language:** [Common / Other — translation required?]
- **Secret Content:** [Hidden message, invisible ink, or coded text — Investigation DC to notice]

> ── ── ── ── ── ── ── ── ── ── ── ──
>
> *[In-world document text written in the voice of the fictional author.
> Uses period-appropriate language matching the world's literary movement.
> If a letter, includes salutation and signature. If a journal, includes
> date and personal tone. If official, includes seals and formal language.
> Redacted or smudged sections marked with [illegible] or [smudged]
> to represent damaged/hidden information.]*
>
> *— [Attribution: who wrote this, when, and why]*
>
> ── ── ── ── ── ── ── ── ── ── ── ──

### ◆ Appendix D: Maps

[Text descriptions of maps with grid references, or references to
generated map images. Include tactical maps for combat encounters
and area maps for exploration.]

### Appendix E: Treasure and Rewards

| Item | Type | Value | Story Connection | Where Found |
|---|---|---|---|---|
| [Name] | [Weapon/Armor/Consumable/etc.] | [GP value] | [Why it matters] | [Location] |

**Experience / Milestones:**
- [XP awards or milestone progression for this quest]

### ◆ Appendix F: Faction Clock Updates

| Faction | Previous Stage | Current Stage | What Changed | Visible to PCs? |
|---|---|---|---|---|
| [Name] | [Stage X] | [Stage Y] | [Action taken] | [Yes/No] |

### Appendix G: DM Contingency Plans

**If PCs skip [location/NPC]:**
[How to deliver critical information another way — portable secrets]

**If PCs go completely off-script:**
[What happens in the world regardless of PC involvement — Living Clock consequences]

**If quest runs long (multi-session):**
[Natural break points where the DM can pause and resume next session]

**If quest resolves quickly:**
[Additional content to extend — optional exploration, NPC scenes, or related hooks]

### ◆ Appendix H: Cross-References

- **Campaign Guide:** See `[campaign-name]-guide.md` for quest board and campaign overview
- **Canon File:** See `[campaign-name]-canon.md` for world state
- **Plot Web:** See `[campaign-name]-plot-web.md` for connection map
- **NPC Details:** See `[world-name]-npcs.md` for full NPC profiles
- **Faction Details:** See `[world-name]-factions.md` for faction info
- **Related Quests:** `[campaign-name]-quest-[related-quest-name].md` — [how they connect]
- **Session Log:** See `[campaign-name]-session-log.md` for play history
```

---

## Module Writing Standards

### Read-Aloud Text Rules

Read-aloud (boxed) text MUST:
- Be written in **second person, present tense** (*"You see..." / "The air grows cold..."*)
- Use **sensory details** — sight, sound, smell, touch, temperature
- Be **3-5 sentences** — long enough to set mood, short enough to not bore
- **Never assume PC actions** — describe the environment, not what PCs do
- **Never reveal hidden information** — only what's immediately apparent

Tag: `[READ-ALOUD: scene name — location]`

### DM Notes Standards

DM Notes (💡 tips) MUST:
- Anticipate the **2-3 most likely player reactions** and provide guidance
- Include **pacing advice** — when to speed up, slow down, or cut
- Suggest **tone adjustments** — how the DM's voice/energy should shift
- Reference **consequences** — what happens if PCs succeed, fail, or avoid
- Be **actionable** — not vague advice, but specific "if X, then Y" guidance
- Include **ambiance cues** — music/sound suggestions for the scene

Tag: `[DM TIP: category — context]`

### NPC Dialogue Standards

NPC dialogue MUST:
- Sound **distinct** — each NPC has recognizable speech patterns
- Serve **double duty** — advance plot AND reveal character
- Include **fallback lines** — what the NPC says if conversation stalls
- Note **lying tells** — if the NPC is deceptive, note subtle cues the DM can play
- Reference **motivation** — why the NPC says what they say

### Encounter Design Standards

Every encounter in a module MUST:
- Pass the **Connection Test** — connected to plot, faction, character, location, theme, or consequence
- Include **scaling notes** — how to adjust for different party sizes/levels
- Describe **environmental storytelling** — the battlefield tells a story
- Provide **multiple resolution paths** — combat is never the only option
- Note **time estimates** — how long this encounter typically takes to run

### Sandbox Signal Language Standards

Module prose MUST use **sandbox-compatible language** that presents situations, never scripts:

**DO say:**
- "The party might..." / "If the party chooses to..."
- "This scene can occur at..." / "DM may place this encounter when..."
- "Possible approaches include..." / "Players may decide to..."
- "This situation is active whether or not the party engages with it."

**DON'T say:**
- "The party will..." / "The players then..."
- "Next, the group goes to..." / "After this, they must..."
- "The correct path is..." / "The party needs to..."

**Portable Elements:** Every module should identify scenes, NPCs, and secrets that are **portable** — they work regardless of where the party goes or what approach they take. Portable elements can be relocated to wherever the party ends up.

See [72-SANDBOX-PREP.md](72-SANDBOX-PREP.md) for the full Sandbox Signal Language reference.

### Treasure and Reward Standards

Every treasure/reward MUST:
- Have a **story connection** — why this item is here, who made it, what it means
- Include **GP value** — for player reference
- Note **mechanical effects** — if magical, full item description
- Reference **player desires** — which PC(s) would want this and why (per Reward Systems)

---

## Module Scope by Campaign Format

### One-Shot (Single Quest Module)
- **Quests:** 1 self-contained quest module + minimal Campaign Guide
- **Length:** 15-25 pages
- **Encounters:** 2-4
- **NPCs:** 3-5 with dialogue
- **Maps:** 1-2 areas
- **Appendices:** A, B, E, G (minimal)
- **Notes:** No quest board needed — the module IS the adventure

### Short Arc (3-8 Quest Modules)
- **Quests:** 3-8 quest modules + Campaign Guide with quest board
- **Length per module:** 10-18 pages
- **Encounters per module:** 1-3
- **NPCs per module:** 3-6 with dialogue
- **Maps:** 1-3 areas per module
- **Appendices:** A-H (full set for complex quests)
- **Campaign Guide** includes quest board with 5-10 quests (not all need full modules — some are sketches for DM improvisation or future development)
- **Quest availability:** Most quests available from the start; 1-2 may have justified prerequisites

### Full Campaign (10+ Quest Modules)
- **Quests:** 10+ quest modules + comprehensive Campaign Guide
- **Length per module:** 12-20 pages
- **Encounters per module:** 2-4
- **NPCs per module:** 4-8 with dialogue
- **Maps:** 2-4 areas per module
- **Appendices:** A-H (full set for every module)
- **Campaign Guide** includes tiered quest board (Tier 1 quests available first, Tier 2-4 unlock as the world state evolves)
- **Every 5 quest modules** — include a Faction Clock summary in the Campaign Guide update
- **Tier transitions** include world-state summaries in the Campaign Guide
- **Quest pool management:** DM always has 3-5 quest modules ready; Architect generates new ones as the pool depletes or the world state creates new situations

---

## Module Generation Workflow

### Step 1: Campaign / Quest Board Planning
Before writing quest modules, establish:
1. What is the campaign's driving force and central tension?
2. What situations, locations, factions, and threats exist in the world?
3. What quests emerge naturally from these elements? (List 5-15 quest concepts)
4. Which quests are immediately available vs. gated by prerequisites?
5. What tier/level range suits each quest?
6. How do the quests connect to each other (shared NPCs, locations, factions)?
7. What Living Clock stages affect quest availability or urgency?

**Output:** Campaign Guide with quest board.

Tag: `[MODULE PLANNING: campaign name — quest board — quest count]`

### Step 2: Quest Design
For each quest module, determine:
1. What is the active situation? (What is happening RIGHT NOW, whether or not the party gets involved?)
2. What is the dramatic question?
3. Who are the key forces in conflict?
4. What approaches can the party take? (Combat, stealth, diplomacy, avoidance)
5. What happens if the party NEVER engages? (Living Clock consequence)
6. What discovery hooks lead the party here? (List 3+ sources)
7. What makes this quest order-independent? (Or, if it has prerequisites, what justifies the gate?)

### Step 3: Full Module Draft
Write the complete quest module following the template structure above. Verify:
- The module works as a standalone adventure
- No assumptions about prior or future sessions
- Multiple entry points and approaches exist
- Discovery hooks provide 3+ ways to learn about this quest
- Portable elements (scenes, NPCs, secrets) are marked

### Step 4: Module Audit
Before delivering, verify:
- [ ] **Order-independence check** — this module works regardless of which quests came before it
- [ ] **No session-number assumptions** — no references to "session 1" or "last session" in the module body
- [ ] **Discovery hooks present** — at least 3 ways the party can learn about this quest
- [ ] **Prerequisite minimization** — this quest has zero prerequisites, or prerequisites are justified and multi-sourced
- [ ] **Portable elements identified** — scenes, NPCs, and secrets that work regardless of party approach
- [ ] **"If avoided" path exists** — the module describes what happens if the party never engages (Living Clock)
- [ ] **Player approach variety** — at least 3 different approaches the party can take, including creative/unexpected
- [ ] Every encounter passes the Connection Test
- [ ] Read-aloud text uses second person, present tense
- [ ] No PC actions are assumed or dictated
- [ ] DM Notes anticipate likely player reactions
- [ ] NPC dialogue is distinct and in-character
- [ ] Treasure has story connections
- [ ] Scaling notes provided for encounters
- [ ] Timing estimates are realistic
- [ ] Cross-references to Campaign Guide and related quests are correct
- [ ] Faction clock updates are tracked
- [ ] Rest opportunities are placed appropriately
- [ ] Ambiance suggestions included for key scenes
- [ ] DM Complexity rating accurately reflects module demands
- [ ] Handouts follow the Handout Generation Standard
- [ ] **Sandbox signal language used** — module presents situations, not scripts ("the party might..." not "the party will...")
- [ ] **Prep depth matches layer** — immediate content is fully detailed, near-term content is sketched, distant content is bullet points

Tag: `[MODULE AUDIT: quest name — pass/fail — issues found]`

### Step 5: Delivery
Present the quest module to the DM with:
- Brief summary of the quest's situation and dramatic question
- Where this quest fits on the quest board (level range, connections)
- Any DM prep notes (voices to practice, props to prepare, handouts to print)
- Ambiance playlist summary (all music/sound cues from the module in order)
- Questions for the DM about customization preferences
- Reminder: **"Run this quest when your players choose to engage with it — not before."**

---

## Module Integration with Campaign Systems

### Tension Architecture
Quest modules are tagged with their tension role in the campaign:
- **Escalation Quest:** Raises the stakes — introduces a new threat, reveals a secret, or advances the opposition's clock
- **Peak Quest:** A major climax — confrontation with a significant antagonist or decision
- **Recovery Quest:** Lower stakes — character development, relationship building, exploration
- **Buildup Quest:** Steady advancement — the party gains resources, allies, or information

The DM selects which quests to offer based on the campaign's current tension needs. The Campaign Guide tracks the overall tension arc across the quest board.

### Discovery Hooks and Quest Seeding
Every quest module lists 3+ discovery hooks. The DM seeds these hooks throughout play:
- **Passive:** Quest board postings, tavern rumors, overheard conversations
- **Active:** NPC requests, faction assignments, personal backstory connections
- **Emergent:** Consequences of other quests, Living Clock events, world changes
- **Accidental:** Travel encounters, exploration finds, random NPC conversations

The DM doesn't "assign" quests — the party chooses what to pursue.

### Living Clock Integration
Quest modules interact with the Living Clock:
- **If quest is completed:** What clock stages advance or halt?
- **If quest is ignored:** What clock stages advance because the situation was not addressed?
- **If quest fails:** What new situations does this create?

The Campaign Guide tracks clock stages and updates quest availability accordingly.

### Fever Dream Doctrine
Every module must pass the "Would You Stream This?" test. If any section would be boring to watch, it must be:
1. Cut entirely, OR
2. Given a story connection, OR
3. Transformed into something memorable

---

## Module vs. Live Session: Key Differences

| Aspect | Pre-Planned Quest Module | Live Session |
|---|---|---|
| **Output** | Quest-named markdown module files + Campaign Guide | Real-time narration + session log |
| **Structure** | Quest/situation-based, order-independent | Sequential, responds to player actions |
| **DM Role** | Selects which module to run based on player choices | Co-facilitates with The Architect |
| **PC Actions** | Anticipated via multiple approaches and contingencies | Responded to in real time |
| **Session Log** | Maintained separately in session log file | Generated per prompt/key event |
| **LLM Markers** | Not used (no ongoing LLM context needed) | Embedded in session logs |
| **Flexibility** | DM adapts on the fly using DM Notes/Contingencies | Architect adapts in real time |
| **Session Identity** | Quests span 1+ sessions; session number is bookkeeping | Each prompt/session is a unit |
| **Best For** | DMs who prep ahead, in-person games, sandbox campaigns | Online play, solo DMs, real-time assistance |

---

## Common Module Mistakes

❌ **Session-numbered modules that assume sequence** — `session-01 → session-02 → session-03` implies linear order
✅ **Quest-named modules that work in any order** — `quest-tower-of-storms.md`, `quest-gnoll-warren.md`

❌ **Assuming prior session outcomes** — "After the party defeated the bandits in the last module..."
✅ **Self-contained situation descriptions** — "The bandit camp has been raiding trade routes. If already dealt with, the camp is abandoned."

❌ **Single discovery hook** — "The NPC tells the party about the quest"
✅ **Multiple discovery hooks** — "The party can learn about this from the quest board, tavern rumors, the merchant NPC, or encountering the wreckage during travel"

❌ **No 'if avoided' path** — Module assumes the party WILL engage
✅ **Living Clock consequences for avoidance** — "If the party never investigates, the situation escalates: the mine collapses, trapping the miners"

❌ **Bullet-point outline instead of prose** — Modules are narratives, not checklists
✅ **Atmospheric read-aloud text with sensory details**

❌ **No DM guidance** — Just describing scenes with no tips
✅ **Inline DM Notes anticipating player reactions and offering solutions**

❌ **Assuming PC actions** — "The party enters the cave and fights the dragon"
✅ **"If the PCs enter the cave, they find..." with alternatives for other choices**

❌ **Generic encounters** — "Fight 4 goblins in a room"
✅ **Story-connected encounters with terrain, tactics, and scaling notes**

❌ **Treasure without story** — Random loot table
✅ **Every treasure item has a narrative reason for being there**

❌ **No timing guidance** — DM can't tell if they're on pace
✅ **Estimated duration for each scene/encounter**

❌ **No ambiance guidance** — DM guesses the mood
✅ **Suggested Ambiance field for every scene with specific sound/music cues**

❌ **No rest pacing** — DM doesn't know when to offer rests
✅ **Rest Opportunity markers with narrative justification**

❌ **Generic handouts** — Plain text with no in-world flavor
✅ **Handouts formatted as in-world documents with condition, authorship, and hidden content**

❌ **Cliffhangers that assume the next module** — "The party must go to the tower next session"
✅ **Quest outcomes that open possibilities** — "The party now knows about the tower, the smuggler's den, and the faction's betrayal — which thread do they pull?"

---

## DM Complexity Rating

Every module header includes a **DM Complexity** rating from ★☆☆☆☆ to ★★★★★ that tells the DM how much preparation effort this specific quest module requires.

### Rating Scale

| Rating | Label | What It Means |
|---|---|---|
| ★☆☆☆☆ | **Straightforward** | Linear flow, minimal NPCs, simple encounters. New DMs can run this cold. |
| ★★☆☆☆ | **Standard** | Some branching, 2-3 NPCs to voice, standard combat. Light prep needed. |
| ★★★☆☆ | **Moderate** | Multiple NPCs with distinct voices, tactical combat, branching paths. Read-through recommended. |
| ★★★★☆ | **Complex** | Heavy roleplay with 4+ voiced NPCs, multi-phase encounters, political intrigue, player handouts. Full read-through required. |
| ★★★★★ | **Demanding** | Requires voice acting range, complex tactical setpieces, multiple simultaneous plot threads, extensive prop/handout prep. DM should rehearse key scenes. |

### Complexity Factors

The rating is determined by the highest-scoring combination of:
- **NPC Voices**: How many distinct NPCs the DM must portray (0-1 = low, 4+ = high)
- **Combat Tactics**: Simple melee vs. multi-phase boss with lair actions (simple = low, multi-phase = high)
- **Branching Paths**: Linear vs. multiple meaningful forks (linear = low, 3+ forks = high)
- **Props/Handouts**: None vs. multiple in-world documents to prepare (none = low, 3+ = high)
- **Emotional Range**: Single tone vs. tonal shifts within the quest (single = low, 3+ shifts = high)
- **Rules Complexity**: Basic checks vs. complex skill challenges or unusual mechanics (basic = low, unusual = high)

Tag: `[DM COMPLEXITY: ★★★☆☆ — justification]`

---

## Session 0 Module Variant

Session 0 is NOT a play session — it is a **setup, negotiation, and character creation session**. It uses a fundamentally different template from play sessions.

### When to Use
- First session of any Short Arc or Full Campaign
- One-shots may skip Session 0 (incorporate into opening 15 minutes)
- When the DM explicitly requests a Session 0

### Session 0 Module File

**File:** `[campaign-name]-session-00-module.md`

### Session 0 Template

```markdown
# [Campaign Name] — Session 0: [Campaign Title] Setup

**Campaign:** [Campaign Name]
**Session:** 0 (Setup)
**Estimated Duration:** [45-90 minutes depending on campaign format]
**DM Complexity:** ★☆☆☆☆ — [Session 0 is collaborative, not performance]
**Campaign Format:** [One-Shot / Short Arc / Full Campaign]

---

## ★ Campaign Pitch

### Read-Aloud: The World

> *[3-5 sentence atmospheric introduction to the world. Sets the
> genre, tone, and central tension without spoilers. This is the
> "back of the book" pitch that gets players excited.]*

### Campaign Overview (DM Eyes Only)
- **Driving Force:** [What drives the STORY]
- **Ending Type:** [Resolved/Unresolved/Ambiguous/Unexpected/Tied/Expanded]
- **Literary Movement:** [Tone/style influence]
- **Tier Range:** [1-4, or subset]
- **Estimated Sessions:** [Number]
- **Themes:** [2-3 major themes]
- **Content Boundaries:** [What WON'T appear in this campaign]

> **💡 DM TIP:** [How much to reveal vs. keep secret. Which details
> build excitement vs. which spoil surprises.]

---

## ★ Safety and Expectations

### Table Ground Rules
- **Session Length:** [Expected duration per session]
- **Frequency:** [Weekly / Biweekly / Monthly]
- **Absence Policy:** [What happens when a player can't attend]
- **Communication:** [How the group communicates between sessions]

### Safety Tools
- **Lines:** [Hard "no" topics that will not appear]
- **Veils:** [Topics handled off-screen or abstractly]
- **Safety Mechanic:** [X-Card / Lines & Veils / Open Door / etc.]

> **💡 DM TIP:** [How to facilitate this conversation without making
> it awkward. Frame as "making the game fun for everyone." Let players
> submit privately if preferred.]

### Tone Negotiation
- **Proposed Tone:** [From eight-tone palette]
- **Discussion Prompts:**
  - *"How dark do you want this to get?"*
  - *"Do you prefer combat-heavy, roleplay-heavy, or balanced?"*
  - *"How do you feel about PvP or inter-party conflict?"*
  - *"Are you here for the story, the tactics, or both?"*

---

## ★ Character Creation Guide

### World Context for Players
[Brief player-facing summary of the world — enough to make informed
character choices. NO DM secrets.]

### Available Options
- **Races/Ancestries:** [Which are common, rare, or restricted in this world]
- **Classes:** [Any thematic guidance — which classes fit naturally]
- **Backgrounds:** [Suggested backgrounds that connect to the world]
- **Starting Level:** [Level and starting equipment rules]

### Character Connection Prompts
Each player should answer:
1. *"Why is your character in [starting location]?"*
2. *"What does your character want more than anything?"*
3. *"What is your character afraid of?"*
4. *"How does your character know at least one other PC?"*

> **💡 DM TIP:** [How to use these answers to create PC-specific hooks.
> Which answers connect to campaign themes. How to weave PC
> backstories into the existing plot web WITHOUT breaking campaign
> independence.]

### Party Dynamics
- **Party Size:** [Expected number of PCs]
- **Role Coverage:** [Suggestions for party balance — not required but helpful]
- **Inter-PC Relationships:** [Encourage pre-established bonds]

---

## ★ World Primer (Player Handout)

[A 1-2 page player-facing document covering:]
- **The World in Brief** — Setting, era, general atmosphere
- **Major Factions** — PUBLIC knowledge only (names, general reputation)
- **The Current Situation** — What everyone knows about the state of affairs
- **Common Knowledge** — Religion, magic, technology, social norms
- **Starting Location** — Where the campaign begins and what it's like

> ── ── ── ── ── ── ── ── ── ── ── ──
>
> *[In-world document: "A Traveler's Guide to [World/Region]" or
> similar framing device that delivers world info as a diegetic
> document players can reference.]*
>
> ── ── ── ── ── ── ── ── ── ── ── ──

---

## ★ Session 0 Wrap-Up

### Character Finalization Checklist
- [ ] All PCs have names, races, classes, and brief identities
- [ ] Each PC has answered the Connection Prompts
- [ ] Inter-PC relationships established
- [ ] PC file (`[campaign-name]-pcs.md`) created

### DM Takeaways
- [ ] Player desires noted (for Reward System)
- [ ] Tone preferences confirmed
- [ ] Safety boundaries recorded
- [ ] Schedule confirmed
- [ ] Any world modifications based on PC backstories

### Teaser for Session 1

> *[2-3 sentence teaser that previews the opening of Session 1
> without spoiling it. Builds anticipation. Ends on a question
> or evocative image.]*

> **💡 DM TIP:** [How to bridge from Session 0 to Session 1.
> What to prep between now and the first play session.]
```

Tag: `[SESSION 0 MODULE: campaign setup — character creation — safety tools]`

---

**See also:**
- [52-LIVE-SESSION-MANAGEMENT.md](52-LIVE-SESSION-MANAGEMENT.md) — Live session alternative
- [70-CAMPAIGN-FORMAT.md](70-CAMPAIGN-FORMAT.md) — Campaign format systems and tension architecture
- [72-SANDBOX-PREP.md](72-SANDBOX-PREP.md) — Sandbox worldbuilding and Lazy DM prep
- [50-ENCOUNTER-COMBAT.md](50-ENCOUNTER-COMBAT.md) — Encounter design rules
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — File naming and directory conventions
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Reward and treasure design
- [91-DM-TIPS-REFERENCE.md](91-DM-TIPS-REFERENCE.md) — DM guidance reference
