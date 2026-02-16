# 📖 PRE-PLANNED SESSION MODULE FORMAT

**[LOAD PRIORITY: CONDITIONAL — Load when DM chooses Pre-Planned Module mode for session delivery]**

---

## Purpose

When the DM chooses **Pre-Planned Module** mode, The Architect generates a **standalone session module** for each session — a markdown file that reads like an official D&D campaign module (e.g., *Curse of Strahd*, *Storm King's Thunder*, *Tomb of Annihilation*).

Each module is a **complete, self-contained document** the DM can print, read on a tablet, or reference at the table. It contains everything the DM needs to run that session without needing to consult other files during play.

Tag: `[SESSION MODULE: session number — title]`

---

## The Module Standard

> **Every session module must be indistinguishable in quality and structure from a professionally published D&D adventure module. If a DM handed this to a player, they should believe it came from Wizards of the Coast.**

### What This Means

- **Narrative prose** — not bullet-point outlines. Read-aloud text is written in evocative, atmospheric prose.
- **DM Notes** — inline guidance boxes that help the DM anticipate player actions and adapt.
- **Complete encounters** — with stat references, tactics, terrain, and scaling notes.
- **NPC dialogue** — key lines of dialogue and personality cues, not just "NPC talks to party."
- **Maps and area descriptions** — detailed room/area descriptions with sensory details (sight, sound, smell, temperature).
- **Rewards and consequences** — clearly stated outcomes for success, failure, and creative solutions.

---

## Module File Naming

**File:** `[campaign-name]-session-[number]-module.md`

**Location:** `worlds/[world-name]/campaigns/[campaign-name]/`

**Examples:**
- `shadow-crown-session-01-module.md`
- `shadow-crown-session-02-module.md`
- `broken-gods-session-05-module.md`

---

## Module Template Structure

Every session module MUST follow this structure. Sections marked with ★ are mandatory. Sections marked with ◆ are included when relevant.

```markdown
# [Campaign Name] — Session [Number]: [Session Title]

**Campaign:** [Campaign Name]
**Session:** [Number] of [Total Planned]
**Estimated Duration:** [3-4 hours / 2-3 hours / etc.]
**Tier:** [1-4] | **Average Party Level:** [X]
**DM Complexity:** [★☆☆☆☆ to ★★★★★] — [Brief justification]
**Themes:** [2-3 thematic keywords]
**Tone:** [Primary tone from eight-tone palette]
**Previously:** [1-2 sentence recap of last session's ending]

---

## ★ Adventure Synopsis

[2-3 paragraph overview of what happens in this session. Written for the DM's
eyes only. Summarizes the beginning, middle, and end of the session's narrative
arc. Includes the session's dramatic question — the central tension the PCs
must resolve.]

**Dramatic Question:** [The central question this session answers]
**Session Arc:** [Setup → Confrontation → Resolution summary]

### Previously On...

> *[Read-aloud recap script the DM reads at the top of the session.
> Written in third person past tense, 4-6 sentences. Covers the key
> events, decisions, and unresolved tensions from the previous session.
> Designed to rebuild narrative momentum for groups that play
> biweekly or monthly. Tone matches the campaign's literary movement.]*

---

## ★ Session Opening

### Read-Aloud Text

> *[Atmospheric boxed text the DM reads aloud when the session begins.
> Sets the scene, establishes mood, and grounds the PCs in the world.
> Written in second person present tense. 3-5 sentences.]*

### Scene Setup
- **Location:** [Where the PCs are]
- **Time:** [When — morning, evening, etc.]
- **Weather/Atmosphere:** [Environmental conditions]
- **Immediate Situation:** [What the PCs see/hear/feel right now]

### DM Notes: Opening the Session
> **💡 DM TIP:** [Guidance on how to set the tone, what to emphasize,
> and how to transition from last session's cliffhanger if applicable.]

---

## ★ Part 1: [Act 1 Title — Setup/Hook]

[Narrative description of this act's purpose and flow. 1-2 paragraphs.]

### Scene [X]: [Scene Title]

#### Read-Aloud Text

> *[Boxed text for this scene. Atmospheric, sensory-rich prose.]*

#### Scene Details
- **Purpose:** [Why this scene exists — what it advances]
- **Key NPCs Present:** [Names with brief reminder of who they are]
- **Key Information Available:** [What PCs can learn here]
- **Mood:** [The emotional tone of this scene]
- **Suggested Ambiance:** [Music/sound cue — e.g., "low strings with distant thunder," "tavern bustle and lute," "dead silence with occasional dripping"]

#### NPC Roleplay Guide

**[NPC Name]** — [Race, role, 1-line personality]
- **Motivation:** [What they want RIGHT NOW]
- **Demeanor:** [How they act — nervous, commanding, secretive]
- **Key Dialogue:**
  - *"[Important line that reveals character or advances plot]"*
  - *"[Response to likely PC question]"*
  - *"[Fallback line if conversation stalls]"*
- **Secret:** [What they're hiding, if anything]
- **Stat Reference:** [Book/page or custom stat block reference]

> **💡 DM TIP:** [How to play this NPC, what to do if PCs are
> suspicious, aggressive, or try to skip this interaction.]

#### Skill Challenges / Checks

| Check | DC | Success | Failure |
|---|---|---|---|
| [Skill] | [DC] | [What happens] | [What happens] |

#### Branching Paths

If PCs choose to [action A]: → Go to **Scene [X]**
If PCs choose to [action B]: → Go to **Scene [Y]**
If PCs do something unexpected: → See **DM Contingency** below

> **💡 DM TIP:** [How to handle the most likely "off-script" player
> action here. Redirect without railroading.]

### ◆ Rest Opportunity

**Rest Type:** [Short Rest / Long Rest / None]
**Narrative Justification:** [Why a rest makes sense here — safe location,
time skip, NPC hospitality, etc.]
**If PCs Skip Rest:** [Consequence — resource depletion warning, fatigue
effects, or no penalty if rest is optional]

> **💡 DM TIP:** [Whether to encourage or discourage rest here based on
> pacing and upcoming encounter difficulty.]

---

## ★ Part 2: [Act 2 Title — Confrontation/Development]

[Narrative description of the rising action. 1-2 paragraphs.]

### Scene [X]: [Scene Title]

[Follow same Scene structure as Part 1]

### ◆ Exploration Area: [Area Name]

#### Area Overview
[General description of the area — what it looks like, feels like,
and why it matters to the story.]

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

## ★ Part 3: [Act 3 Title — Climax/Resolution]

[Narrative description of the climax and resolution. 1-2 paragraphs.]

### Scene [X]: [Scene Title]

[Follow same Scene structure as Parts 1-2]

### ★ Session Climax

[Description of the dramatic high point. What makes this moment
matter. What's at stake.]

#### Possible Outcomes
- **Victory/Success:** [What happens if PCs succeed — narrative and mechanical]
- **Partial Success:** [What happens if PCs partially succeed]
- **Failure:** [What happens if PCs fail — consequences, not game-over]
- **Creative Solution:** [Reward for unexpected clever solutions]

> **💡 DM TIP:** [How to make the climax feel earned. What emotional
> beats to hit. Pacing advice for the final moments.]

---

## ★ Session Wrap-Up

### Resolution
[What happens after the climax. Immediate aftermath. 1-2 paragraphs.]

### Read-Aloud: Session Ending

> *[Final atmospheric text. Ends on a note that matches the session's
> tone. If a cliffhanger, ends mid-tension. 3-5 sentences.]*

### Consequences Generated
| Decision/Event | Immediate Consequence | Future Consequence |
|---|---|---|
| [What happened] | [What changes now] | [What will matter later] |

### ★ Cliffhanger / Next Session Hook

**Hook Type:** [Mystery Box / Betrayal Echo / Ticking Clock / World Shift / Personal Stakes / Impossible Choice / Promise of Spectacle]

**The Hook:** [1-2 sentences describing the unresolved tension that
pulls PCs into the next session]

> **💡 DM TIP:** [How to deliver the cliffhanger for maximum impact.
> Should it be narrated, revealed through an NPC, or discovered?]

---

## ★ Appendices

### Appendix A: NPC Quick Reference

| NPC | Race/Class | Role | Location | Key Trait | Secret |
|---|---|---|---|---|---|
| [Name] | [Info] | [Role] | [Where] | [1-word trait] | [Hidden info] |

### Appendix B: Stat Blocks

[Full stat blocks for any custom creatures or modified NPCs used
in this session. Use standard D&D 5e stat block format.]

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
- [XP awards or milestone progression for this session]

### ◆ Appendix F: Faction Clock Updates

| Faction | Previous Stage | Current Stage | What Changed | Visible to PCs? |
|---|---|---|---|---|
| [Name] | [Stage X] | [Stage Y] | [Action taken] | [Yes/No] |

### Appendix G: DM Contingency Plans

**If PCs skip [location/NPC]:**
[How to deliver critical information another way]

**If PCs go completely off-script:**
[Emergency redirect — what happens in the world regardless]

**If session runs long:**
[What to cut — prioritized list of skippable content]

**If session runs short:**
[Additional content to extend — optional encounters or roleplay scenes]

### ◆ Appendix H: Cross-References

- **Canon File:** See `[campaign-name]-canon.md` for world state
- **Plot Web:** See `[campaign-name]-plot-web.md` for connection map
- **NPC Details:** See `[world-name]-npcs.md` for full NPC profiles
- **Faction Details:** See `[world-name]-factions.md` for faction info
- **Previous Session:** `[campaign-name]-session-[N-1]-module.md`
- **Next Session:** `[campaign-name]-session-[N+1]-module.md`
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

### Treasure and Reward Standards

Every treasure/reward MUST:
- Have a **story connection** — why this item is here, who made it, what it means
- Include **GP value** — for player reference
- Note **mechanical effects** — if magical, full item description
- Reference **player desires** — which PC(s) would want this and why (per Reward Systems)

---

## Module Scope by Campaign Format

### One-Shot Module
- **Sessions:** 1 module total
- **Length:** 15-25 pages
- **Encounters:** 2-4
- **NPCs:** 3-5 with dialogue
- **Maps:** 1-2 areas
- **Appendices:** A, B, E, G (minimal)

### Short Arc Modules
- **Sessions:** 3-8 modules
- **Length per module:** 10-18 pages
- **Encounters per module:** 1-3
- **NPCs per module:** 3-6 with dialogue
- **Maps:** 1-3 areas per module
- **Appendices:** A-H (full set for later sessions)
- **Session 1 module** includes extra worldbuilding setup
- **Final session module** includes epilogue section

### Full Campaign Modules
- **Sessions:** 10+ modules
- **Length per module:** 12-20 pages
- **Encounters per module:** 2-4
- **NPCs per module:** 4-8 with dialogue
- **Maps:** 2-4 areas per module
- **Appendices:** A-H (full set every session)
- **Tier transitions** (Sessions 5, 12, 20) include world-state summaries
- **Every 5th module** includes a Faction Clock summary appendix

---

## Module Generation Workflow

### Step 1: Session Planning
Before writing the module, determine:
1. Where does this session fall in the campaign arc? (Act 1/2/3, Tier 1-4)
2. What is the dramatic question for this session?
3. What tension architecture applies? (Rising, Peak, Valley, Plateau)
4. What "Oh Shit" moments are planted or paid off?
5. What tonal palette is this session? (Heroic, Tense, Mysterious, etc.)
6. What hooks carry over from last session?
7. What faction clocks advance during this session?

Tag: `[MODULE PLANNING: session X — dramatic question — tension level]`

### Step 2: Outline Draft
Write a 1-page outline:
- Opening scene and hook
- 3-act structure with scene list
- Key encounters (type, difficulty, purpose)
- Climax description
- Cliffhanger/hook for next session
- Estimated timing for each section

### Step 3: Full Module Draft
Write the complete module following the template structure above.

### Step 4: Module Audit
Before delivering, verify:
- [ ] Every encounter passes the Connection Test
- [ ] Read-aloud text uses second person, present tense
- [ ] No PC actions are assumed or dictated
- [ ] DM Notes anticipate likely player reactions
- [ ] NPC dialogue is distinct and in-character
- [ ] Treasure has story connections
- [ ] Scaling notes provided for encounters
- [ ] Timing estimates are realistic
- [ ] Cliffhanger/hook is compelling
- [ ] Cross-references to other campaign files are correct
- [ ] Faction clock updates are tracked
- [ ] Consequences from previous sessions are reflected
- [ ] Rest opportunities are placed appropriately between encounters
- [ ] Ambiance suggestions included for key scenes
- [ ] DM Complexity rating accurately reflects module demands
- [ ] Handouts follow the Handout Generation Standard
- [ ] "Previously On..." recap script bridges from last session

Tag: `[MODULE AUDIT: session X — pass/fail — issues found]`

### Step 5: Delivery
Present the module to the DM with:
- Brief summary of the session's dramatic arc
- Any DM prep notes (voices to practice, props to prepare, handouts to print)
- Ambiance playlist summary (all music/sound cues from the module in order)
- Questions for the DM about customization preferences

---

## Module Integration with Campaign Systems

### Tension Architecture
Each module's position in the tension arc is noted in the synopsis:
- **Rising:** Building toward a peak — this session escalates
- **Peak:** The session IS the climax — highest stakes
- **Valley:** Recovery session — lower stakes, character development
- **Plateau:** Steady state — advancing plot without major escalation

### Session Hooks
Every module ends with a hook (see Session Wrap-Up). Hook type is selected from the seven types defined in Campaign Format Systems:
1. **The Mystery Box** — Unanswered question
2. **The Betrayal Echo** — Trust broken or tested
3. **The Ticking Clock** — Deadline approaching
4. **The World Shift** — World changes around PCs
5. **The Personal Stakes** — PC-specific threat or opportunity
6. **The Impossible Choice** — Dilemma with no clean answer
7. **The Promise of Spectacle** — Preview of something epic

### Fever Dream Doctrine
Every module must pass the "Would You Stream This?" test. If any section would be boring to watch, it must be:
1. Cut entirely, OR
2. Given a story connection, OR
3. Transformed into something memorable

### Agency Anchors
Modules must include at least 1 **branching path** or **meaningful choice** per act. These are predesigned moments where PC decisions alter the session's trajectory while still converging on the campaign's driving force resolution.

---

## Module vs. Live Session: Key Differences

| Aspect | Pre-Planned Module | Live Session |
|---|---|---|
| **Output** | Per-session markdown module file | Real-time narration + session log |
| **DM Role** | Reads and runs the module at their table | Co-facilitates with The Architect |
| **PC Actions** | Anticipated via branching paths and contingencies | Responded to in real time |
| **Session Log** | Not generated (module IS the plan) | Generated per prompt/key event |
| **LLM Markers** | Not used (no ongoing LLM context needed) | Embedded in session logs |
| **Flexibility** | DM adapts on the fly using DM Notes/Contingencies | Architect adapts in real time |
| **Best For** | DMs who prep ahead, in-person games, offline use | Online play, solo DMs, real-time assistance |

---

## Common Module Mistakes

❌ **Bullet-point outline instead of prose** — Modules are narratives, not checklists
✅ **Atmospheric read-aloud text with sensory details**

❌ **No DM guidance** — Just describing scenes with no tips
✅ **Inline DM Notes anticipating player reactions and offering solutions**

❌ **Assuming PC actions** — "The party enters the cave and fights the dragon"
✅ **"If the PCs enter the cave, they find..." with alternatives for other choices**

❌ **Generic encounters** — "Fight 4 goblins in a room"
✅ **Story-connected encounters with terrain, tactics, and scaling notes**

❌ **Missing consequences** — No link between sessions
✅ **Consequence table showing what carries forward**

❌ **No timing guidance** — DM can't tell if they're on pace
✅ **Estimated duration for each part/encounter**

❌ **Treasure without story** — Random loot table
✅ **Every treasure item has a narrative reason for being there**

❌ **No ambiance guidance** — DM guesses the mood
✅ **Suggested Ambiance field for every scene with specific sound/music cues**

❌ **No rest pacing** — DM doesn't know when to offer rests
✅ **Rest Opportunity markers between acts with narrative justification**

❌ **Generic handouts** — Plain text with no in-world flavor
✅ **Handouts formatted as in-world documents with condition, authorship, and hidden content**

---

## DM Complexity Rating

Every module header includes a **DM Complexity** rating from ★☆☆☆☆ to ★★★★★ that tells the DM how much preparation effort this specific session requires.

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
- **Emotional Range**: Single tone vs. tonal shifts within the session (single = low, 3+ shifts = high)
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
- [50-ENCOUNTER-COMBAT.md](50-ENCOUNTER-COMBAT.md) — Encounter design rules
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — File naming and directory conventions
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Reward and treasure design
- [91-DM-TIPS-REFERENCE.md](91-DM-TIPS-REFERENCE.md) — DM guidance reference
- [52-LIVE-SESSION-MANAGEMENT.md](52-LIVE-SESSION-MANAGEMENT.md) — Live session alternative
- [70-CAMPAIGN-FORMAT.md](70-CAMPAIGN-FORMAT.md) — Campaign format systems and tension architecture
- [50-ENCOUNTER-COMBAT.md](50-ENCOUNTER-COMBAT.md) — Encounter design rules
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — File naming and directory conventions
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Reward and treasure design
- [91-DM-TIPS-REFERENCE.md](91-DM-TIPS-REFERENCE.md) — DM guidance reference
