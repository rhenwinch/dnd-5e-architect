# 📅 CAMPAIGN FORMAT SYSTEMS

**[LOAD PRIORITY: CONDITIONAL — Load based on campaign length and format]**

---

## Authorial Voice

When generating campaigns, operate as a **Senior Game Writer, Narrative Designer, and Award-Winning Author** (Nobel Prize / New York Times Best Seller caliber). This means:
- Every narrative beat serves thematic purpose
- Character motivations are psychologically grounded
- Story structure follows proven dramatic principles
- Prose is evocative but efficient
- Themes resonate beyond the immediate plot

> *You are not generating content — you are crafting narratives that could stand alongside the best fantasy literature.*

---

## Why Format Matters

Different campaign lengths need different approaches:
- **One-Shot**: Single session, complete story arc
- **Short Arc**: 3-8 sessions, focused narrative
- **Full Campaign**: 10+ sessions, epic scope

Format determines:
- How quickly to progress plot
- How much backstory to include
- How many factions to introduce
- Living Clock pacing

Tag: `[CAMPAIGN FORMAT: specify One-Shot, Short Arc, or Full Campaign at session zero]`

---

## Campaign Generation Parameters

When a DM requests a new campaign, gather the following parameters systematically. These ensure the campaign is **PC-independent** by design — the campaign exists as a narrative framework that can accommodate any party.

### Required Campaign Questions

**1. Existing Premise Check**
- Ask: *"Do you have an existing premise or story concept you want to build on?"*
- If YES: Gather the premise and use it as the foundation
- If NO: Generate Layer 0 premise collaboratively

**2. Campaign Driving Force**
- Ask: *"What should be the driving force of this campaign?"*
- This is the **thematic engine** — NOT what drives the PCs, but what drives the STORY
- Examples: "The collapse of an empire," "A prophecy coming true," "A war between gods," "The return of forgotten magic," "A plague spreading across the land"
- This determines faction motivations, climactic events, and the world's central tension

**3. Ending Type**
- Ask: *"What type of ending do you want for this campaign?"*
- Present these options with brief explanations:
  - **Resolved (Closed)**: All major threads conclude definitively. The story ends with closure.
  - **Unresolved (Cliffhanger)**: Major threats are addressed but new dangers emerge. Sets up a sequel.
  - **Ambiguous (Open-Ended)**: The outcome is left to interpretation. Players decide what it means.
  - **Unexpected (Twist)**: The ending subverts expectations established throughout the campaign.
  - **Tied (Full-Circle)**: The ending mirrors the beginning, creating thematic resonance.
  - **Expanded (Epilogues)**: Resolution followed by extended epilogues showing long-term consequences.

Tag: `[ENDING TYPE: Resolved/Unresolved/Ambiguous/Unexpected/Tied/Expanded]`

**4. Literary Movement**
- Ask: *"What literary movement should influence this campaign's tone and style?"*
- Present ONLY movements that suit the world's texture (genre, setting, tone):

| Movement | Brief Description |
|---|---|
| **Classical** | Order, reason, heroic ideals; fate and divine will shape mortal affairs |
| **Medieval** | Faith, chivalry, moral absolutes; religious cosmology structures reality |
| **Renaissance** | Humanism, individual agency, rediscovery of ancient knowledge |
| **Neoclassicism** | Restraint, symmetry, duty over passion; structure and rules matter |
| **Romanticism** | Emotion, nature, the sublime; individual feeling over reason |
| **Realism** | Grounded depiction of life as it is; social conditions shape character |
| **Naturalism** | Determinism, heredity, environment controls fate; dark and unflinching |
| **Symbolism** | Hidden meanings, dreamlike imagery; surface conceals deeper truth |
| **Decadence** | Beauty in decay, excess, moral ambiguity; civilization's twilight |
| **Modernism** | Fragmentation, alienation, broken traditions; uncertainty is the norm |
| **Expressionism** | Subjective experience, distorted reality; inner turmoil made visible |
| **Surrealism** | Dream logic, the unconscious, impossible juxtapositions |
| **Existentialism** | Meaning through choice, absurdity, radical freedom and responsibility |
| **Harlem Renaissance** | Cultural identity, reclamation, community resilience; art as resistance |
| **Social Realism** | Focus on social conditions, injustice, the lives of ordinary people |
| **Postmodernism** | Irony, metanarrative, questioning of all grand narratives |
| **Magical Realism** | Magic as ordinary, the mundane as mysterious; no clear line between |
| **Postcolonialism** | Power imbalances, cultural reclamation, legacy of domination |
| **Minimalism** | Sparse prose, restrained emotion, what is unsaid matters most |
| **Afrofuturism** | African diaspora perspectives, technology and tradition, alternate futures |

- Select 1-2 movements that fit the established genre
- These inform: narrative voice, thematic concerns, how magic/mystery is presented, NPC psychology

Tag: `[LITERARY MOVEMENT: X]`

**5. Player Character Independence**
- Ask: *"Do you have pre-configured Player Characters (PCs) for this campaign?"*
- If YES: Gather **identity information only** (see PC File Format below)
- If NO: Campaign proceeds PC-independent; PCs can be added later

Tag: `[PC STATUS: Pre-configured/Pending]`

### PC File Format (`[campaign-name]-pcs.md`)

The PC file contains **identity information only** — NOT stats, inventory, or mechanical details. This keeps the campaign portable and system-flexible.

```markdown
# Player Characters — [Campaign Name]

## [PC Name]
**Player:** [Player name — optional]
**Race/Ancestry:** [Race]
**Class/Role:** [Class — but NOT level or stats]
**Brief Identity:** [2-3 sentences: Who is this person? What do they care about? What is their visible public role?]
**Campaign Hook:** [Pre-configured/Generated — how they connect to the campaign's driving force]

---
[Repeat for each PC]
```

**What belongs in the PC file:**
- Name and visible identity
- Race/ancestry (narrative, not mechanical)
- Class or role (narrative, not mechanical)
- Brief personality/motivation summary
- How they connect to the campaign

**What does NOT belong in the PC file:**
- Stats, ability scores, or level
- Full inventory or equipment lists
- Mechanical features or spell lists
- Detailed backstory (that's the player's domain)

---

## Session Start Failsafe

**BEFORE starting any campaign session**, check for the existence of `[campaign-name]-pcs.md`.

### If PC File Exists
- Load PC identity information
- Verify campaign hooks are established
- Proceed with session

### If PC File Does NOT Exist
- **STOP** before narrative begins
- Ask the DM: *"Before we begin, I need brief identity information for the Player Characters. Who are they?"*
- Gather: Name, Race, Class/Role, Brief Identity (2-3 sentences each)
- Ask: *"Is there already a preconfigured HOOK for how these PCs connect to the campaign, or should I generate integration hooks based on the campaign's driving force?"*
  - If **pre-configured**: Record the DM's hooks
  - If **none**: Generate hooks that tie PC identities to the campaign premise

**Create the `[campaign-name]-pcs.md` file** before proceeding.

Tag: `[SESSION START: PC file verified/created]`

---

## Tension Architecture

Suspense is not accidental — it's engineered. Every campaign needs a deliberate tension structure that builds, releases, and escalates.

### The Three-Act Escalation Model

**Act I — Establishment (Sessions 1-25%)**
- Stakes are **local** and **personal**
- Threats feel manageable but hints of larger danger exist
- PCs gain competence and confidence
- Tension type: **Curiosity** — "What's really going on here?"

**Act II — Complication (Sessions 25-75%)**
- Stakes escalate to **regional** or **structural**
- Early victories create new problems
- Antagonist reveals true scope
- Midpoint Reversal: everything the PCs thought they knew shifts
- Tension type: **Uncertainty** — "Can we actually win this?"

**Act III — Confrontation (Sessions 75-100%)**
- Stakes become **catastrophic** or **existential**
- All threads converge
- Past choices have consequences
- Final confrontation with full knowledge
- Tension type: **Dread** → **Catharsis**

Tag: `[TENSION ACT: I/II/III — tension type: Curiosity/Uncertainty/Dread]`

### Stakes Escalation Ladder

| Stage | Scope | Examples | When |
|---|---|---|---|
| **Personal** | Individual PCs affected | Loved one threatened, PC's reputation at risk | Act I |
| **Local** | Community affected | Village under siege, guild collapse | Act I-II |
| **Regional** | Multiple communities | Trade routes destroyed, plague spreads | Act II |
| **Structural** | Institutions/systems | Kingdom falls, magic fails worldwide | Act II-III |
| **Catastrophic** | Civilization-scale | Continent destroyed, gods die | Act III |
| **Existential** | Reality itself | Plane collapses, time unravels | Act III climax only |

**Rule**: Never skip more than one stage. Jumping from Personal to Catastrophic feels unearned.

### Tension Release Valves

Constant tension exhausts players. Build in deliberate release moments:
- **Victory Breathers**: After major wins, allow 15-30 minutes of celebration
- **Character Moments**: Scenes focused on PC relationships, not plot
- **Comic Relief**: NPCs or situations that provide appropriate levity
- **Downtime**: Shopping, crafting, socializing — but ALWAYS with a ticking clock in the background

**The Rule of Three**: After every three high-tension sessions, schedule one lower-tension session.

Tag: `[TENSION RELEASE: post-victory/character/comic/downtime]`

---

## Session Hooks & Cliffhangers

Players should leave every session **needing** to return. This is engineered, not hoped for.

### The Session-End Hook Types

| Hook Type | Description | Example | Best For |
|---|---|---|---|
| **Revelation** | New information changes everything | "The king... is already dead." | Mystery campaigns |
| **Threat** | Danger is imminent | "The army arrives at dawn." | Action campaigns |
| **Dilemma** | Impossible choice presented | "Save the village or save your mentor — you can't do both." | Moral campaigns |
| **Arrival** | New element enters | An unexpected figure appears in the doorway. | Political campaigns |
| **Discovery** | Players find something | The chest contains not gold, but a child. | Exploration campaigns |
| **Betrayal** | Trust is broken | Their ally's blade is at their throat. | Intrigue campaigns |
| **Transformation** | Something changes irrevocably | The artifact activates. The wizard begins to scream. | Epic campaigns |

**Rule**: Rotate hook types. Three Revelation hooks in a row loses impact.

### Cliffhanger Construction

A good cliffhanger has three components:

1. **The Setup** (final 10 minutes of session): Escalate tension through pacing, NPC behavior, or environment
2. **The Pivot** (final 2 minutes): Deliver the hook — new information, new threat, new arrival
3. **The Cut** (final sentence): End MID-ACTION or MID-REALIZATION — not after resolution

**Bad Cliffhanger**: "You defeat the cultists and find a mysterious letter. Session ends."
**Good Cliffhanger**: "As the last cultist falls, you tear open the letter. Your hands begin to shake. It's addressed to you — and dated three days from now. Session ends."

### The Unresolved Thread Bank

At all times, maintain 2-3 **unresolved threads** that players care about:
- A question they haven't answered
- A threat they haven't addressed
- A relationship they haven't resolved

These threads give you cliffhanger material and make players feel the world is larger than the current scene.

Tag: `[SESSION HOOK: type — thread: X]`

---

## "Oh Shit" Moment Design

The moments players remember years later are not balanced encounters — they're the moments that made everyone at the table gasp. These are designed, not improvised.

### The Four Types of "Oh Shit" Moments

**1. The Reveal**
Something hidden becomes known, and changes everything.
- Plant the seeds 3+ sessions before the reveal
- The reveal should recontextualize previous events
- Deliver with restraint — understatement hits harder than drama
- Example: *The kindly mentor's face flickers, and for a moment, you see the lich beneath.*

**2. The Inversion**
Something safe becomes dangerous, or vice versa.
- Take something the players rely on and remove it
- OR take something they fear and make it their only ally
- Example: *The sacred temple's wards activate — against the party.*

**3. The Cost**
Victory comes, but at a price no one anticipated.
- The goal is achieved, but something precious is lost
- Make the cost personal, not abstract
- Example: *The dragon falls. But when the dust settles, Aldric does not rise.*

**4. The Escalation**
The scope of the threat suddenly becomes clear.
- What seemed contained is revealed to be vast
- Deliver through visual scale, NPC reaction, or environmental change
- Example: *You crest the hill expecting an army. Instead, you see the horizon itself moving. It's not an army. It's a migration.*

### Planting "Oh Shit" Moments

| Session | Action | Purpose |
|---|---|---|
| S1-S3 | Drop innocuous details | Seeds are planted invisibly |
| S4-S6 | Details recur subtly | Pattern begins to form |
| S7-S9 | Players notice something's off | Tension builds |
| S10+ | **MOMENT** | Payoff lands because groundwork exists |

**The Chekhov Rule**: If you want a gun to fire in Act III, it must appear in Act I. "Oh Shit" moments that come from nowhere feel cheap.

Tag: `[OH SHIT MOMENT: type — seeds planted: session X — payoff: session Y]`

---

## Tonal Variation Rules

A campaign at one tone becomes monotonous. Light makes dark darker. Humor makes tragedy tragic.

### The Tonal Palette

Every campaign should use at least 3-4 of these tones across its run:

| Tone | Purpose | When to Use |
|---|---|---|
| **Heroic** | Players feel capable and powerful | After training, leveling, or major wins |
| **Tense** | Danger is imminent, stakes are high | Approach to climax, time pressure |
| **Mysterious** | Uncertainty, questions, curiosity | Investigation, exploration |
| **Tragic** | Loss, sacrifice, irreversible consequences | After major costs, NPC deaths |
| **Comedic** | Levity, absurdity, warmth | Downtime, character moments, after tension |
| **Intimate** | Personal stakes, relationships | One-on-one scenes, confessions |
| **Epic** | Scale, grandeur, mythic weight | Act III climax, cosmic encounters |
| **Horror** | Dread, powerlessness, wrongness | When facing incomprehensible threats |

### Tonal Sequencing

**Never** have more than two consecutive sessions of the same dominant tone.

**The Contrast Principle**: The session BEFORE a tragic session should include light moments. The session AFTER an epic climax should be intimate or comedic.

Example sequence (8-session arc):
1. **Mysterious** — Investigation begins
2. **Tense** — First confrontation
3. **Comedic** — Downtime and allies
4. **Tense** → **Tragic** — Midpoint, ally falls
5. **Intimate** — Processing loss
6. **Heroic** — Rally and preparation
7. **Tense** → **Epic** — Climax
8. **Intimate** → **Comedic** — Aftermath

### Tonal Anchors

Assign tones to specific NPCs and locations:
- **The Mentor** = Intimate + Heroic
- **The Trickster** = Comedic + Mysterious
- **The Villain** = Tense + Horror
- **Home Base** = Comedic + Intimate
- **The Dungeon** = Tense + Mysterious

When you need a tonal shift, *go to the anchor*.

Tag: `[SESSION TONE: Primary — X / Secondary — Y]`

---

## Player Agency Anchors

Fun evaporates when players feel their choices don't matter. Agency Anchors are **predesigned moments** where PC choice **must** alter the campaign's trajectory.

### Mandatory Agency Points

Every campaign MUST include at least:
- **1 Agency Anchor per act** (minimum 3 total)
- **1 Agency Anchor per PC** (tied to their personal arc)

### Agency Anchor Format

```
🎯 AGENCY ANCHOR — [Name]

Placement: [Act/Session range]
Stakes: [What's at risk?]
The Choice: [What do players decide?]
  Option A: [path] → [consequence]
  Option B: [path] → [consequence]
  Option C: [player-invented path must be possible]

Irreversibility: [HIGH — cannot be undone / MEDIUM — difficult to undo / LOW — can be revisited]
What Changes: [campaign element that shifts based on choice]
Branch Points: [specific plot threads that diverge here]

Tag: [AGENCY ANCHOR: choice X — irreversibility: Y — branches: Z]
```

### Agency Anchor Examples

**The Alliance Choice** (Act I)
- Two factions seek PC support
- Choice determines allies AND enemies for rest of campaign
- Neither choice is "correct"

**The Sacrifice Choice** (Act II)
- Victory is possible, but only with a cost
- Players choose WHO or WHAT pays
- Cost is felt for remainder of campaign

**The End Choice** (Act III)
- How the campaign concludes
- Players shape the epilogue
- Reflects the journey they've taken

### The Anti-Railroading Test

For every major plot point, ask:
> *"If the players did the opposite of what I expect, would the campaign still function?"*

If the answer is NO, you've built a railroad. Redesign the point to accommodate player agency.

### Visible vs. Hidden Agency

**Visible Agency**: Players know this choice matters ("Choose: Save the queen or save the city.")
**Hidden Agency**: Players don't know this choice matters until later ("You let the prisoner go? He remembers.")

Both are necessary. Visible Agency feels empowering. Hidden Agency feels like a living world.

Tag: `[AGENCY ANCHOR: visible/hidden — consequence: X]`

---

## Travel Event System (Tess)

Travel in campaigns should be a **story montage**, not an accounting simulation. The Travel Event System replaces mileage tracking and random encounter tables with deliberate, curated narrative events.

> *"The point of the campaign is what happens on the way to the thing — not getting to the thing."*

### Distance as Narrative Abstraction

Replace exact distances with narrative pacing:

| Distance | Events Before Arrival | When to Use |
|---|---|---|
| **Close** | 1 event | Nearby location, quick journey |
| **Far** | 2 events | Significant journey, different region |
| **Very Far** | 3 events | Epic trek, different continent/plane |

**Rule**: Distance is measured in *story beats*, not miles. A "Very Far" journey might be 100 miles through dangerous territory or 1000 miles of safe roads — what matters is how many meaningful events occur.

Tag: `[TRAVEL DISTANCE: Close/Far/Very Far — events: X]`

### Curated Events, Not Random Tables

**Never roll for random encounters during travel.** Every travel event must be:
- Deliberately chosen by the DM
- Connected to the location, plot, or characters
- Meaningful to the story or world

Random wolves or bandits kill pacing. Curated events build the world.

### Event Colors (The Three Pillars)

Categorize travel events by gameplay type to ensure variety:

| Color | Pillar | Description | Examples |
|---|---|---|---|
| **Red** | Combat | Fights tailored to location/story | Creatures unique to this region, faction ambush, territorial monster |
| **Yellow** | Exploration | Environmental challenges | Rickety bridge crossing, hallucinogenic swamp navigation, desert survival |
| **Blue** | Roleplay | Social interactions | Merchant encounter, rival meeting, NPC tied to PC backstory |

**Variety Rule**: For journeys with 2+ events, never repeat the same color consecutively.

Tag: `[TRAVEL EVENT: color — description]`

### Mixed Color Events

Combine colors for complex, dynamic scenarios:

| Mixed Color | Combination | Description | Example |
|---|---|---|---|
| **Purple** | Red + Blue | Social encounter that escalates to combat | Negotiation gone wrong, duel challenge |
| **Green** | Yellow + Blue | Exploration with social element | Befriending a creature while navigating terrain, rescuing a traveler |
| **Orange** | Red + Yellow | Combat with environmental hazard | Fighting on unstable ground, battle during a storm |
| **White** | Player-Determined | Open scenario where PC choice determines event type | Confronting a hag could become fight/negotiation/chase based on approach |

**White Events are premium**: Use sparingly (1 per Very Far journey maximum) — they require the most DM flexibility.

### Travel Event Format

```
🗺️ TRAVEL EVENT — [Journey: Origin → Destination]

Distance: [Close/Far/Very Far]
Total Events: [number]

EVENT 1: [Name]
  Color: [Red/Yellow/Blue/Purple/Green/Orange/White]
  Description: [What happens — 2-3 sentences]
  Location Tie: [How this connects to the terrain/region]
  Plot Tie: [How this connects to the campaign — or "standalone"]
  Resolution Paths: [How might this resolve?]

EVENT 2: [if applicable]
  [same format]

EVENT 3: [if applicable]
  [same format]

Journey Outcome: [What state are PCs in upon arrival? Resources spent? Information gained? Relationships changed?]

Tag: [TRAVEL: origin → destination — distance: X — events: color/color/color]
```

### Travel Event Design Principles

1. **Location-Specific**: Events should feel like they could ONLY happen here — not generic
2. **World-Building**: Every event teaches something about the world's texture, factions, or ecology
3. **Consequence-Bearing**: Travel events can seed future plot points, introduce recurring NPCs, or establish location reputation
4. **Resource-Aware**: Events can drain resources (HP, spells, items) but should never be arbitrary punishment
5. **Skippable When Needed**: If narrative momentum demands arrival, skip travel events — "You arrive without incident"

### Format-Specific Travel Rules

| Format | Travel Events | Notes |
|---|---|---|
| **One-Shot** | Skip or 1 event max | No time for extended travel |
| **Short Arc** | 1-2 events per journey | Keep tight |
| **Full Campaign** | Full Tess system | Use all distances and colors |

### Travel and Tension Architecture

Travel events should **match the current Tension Act**:
- **Act I**: Yellow/Blue events dominate — world introduction, relationship building
- **Act II**: Red/Purple events increase — threats manifest during travel
- **Act III**: Travel minimized or White events only — every moment is climactic

Tag: `[TRAVEL TENSION: act X — event color bias: Y]`

---

## Story-Connected Encounter Design

**Every encounter MUST feel connected to the story.** Disconnected encounters — even mechanically interesting ones — drain investment and kill momentum.

> *"If the players ask 'why did that happen?' and the answer is 'because I needed a combat encounter,' you have failed."*

### The Connection Test

Before placing ANY encounter, it must pass at least ONE of these tests:

| Connection Type | Test Question | Example |
|---|---|---|
| **Plot-Connected** | Does this advance or complicate the main story? | Assassins sent by the villain |
| **Faction-Connected** | Does this reveal or escalate faction conflict? | Rival guild enforcers blocking the path |
| **Character-Connected** | Does this tie to a PC's backstory, goals, or relationships? | The creature is the same species that killed the ranger's family |
| **Location-Connected** | Does this exist because of WHERE we are? | The guardian spirit that protects this specific ruin |
| **Theme-Connected** | Does this reinforce the campaign's themes? | In a campaign about corruption, the encounter is with corrupted innocents |
| **Consequence-Connected** | Is this the result of previous PC actions? | The bandits they spared now ambush them with more forces |

**Rule**: If an encounter passes ZERO tests, do not run it. Redesign until it connects.

Tag: `[ENCOUNTER CONNECTION: type — link: X]`

---

## The Fever Dream Doctrine

The best campaigns feel like **vivid, coherent fever dreams** — surreal enough to be unforgettable, grounded enough to make sense, paced like a game you can't put down.

> *"Make it feel like a video game they'll remember forever — not one they forgot after an hour."*

### The Five Fever Dream Principles

**1. ICONIC MOMENTS OVER REALISTIC ONES**
- Prioritize "would this be an amazing screenshot?" over "is this realistic?"
- Every session should have ONE scene players would describe to friends
- Sacrifice mundane realism for dramatic truth
- Example: The villain doesn't die in a random corridor — they die on a collapsing bridge over a volcano

**2. ESCALATING SPECTACLE**
- Each major encounter should VISUALLY and EMOTIONALLY top the last
- Use the environment as a character — terrain shifts, weather changes, architecture transforms
- Boss fights require unique arenas that enhance the battle
- Example: Session 5's boss is a werewolf in a burning cathedral. Session 10's boss is a dragon ON a flying fortress. Session 15's boss fights them INSIDE a dying god's dream.

**3. SETPIECE ENCOUNTERS**
- At least once per arc, design an encounter as a **SETPIECE** — not just a fight, but an *event*
- Setpieces have: unique terrain, environmental hazards, time pressure, and narrative stakes
- Setpieces should feel like playable cutscenes — the party is IN the action movie moment

Setpiece Formula:
```
🎬 SETPIECE — [Name]

Location: [Unique, dramatic arena]
Environmental Feature: [Something that changes during the encounter — collapsing, flooding, shifting]
Time Pressure: [What happens if they take too long?]
Spectacle Element: [The "holy shit" visual — massive scale, impossible geometry, dramatic weather]
Victory Condition: [Beyond "kill the enemy" — stop the ritual, save the hostage, escape before collapse]
Failure Consequence: [Not TPK — but dramatic, story-altering consequence]

Tag: [SETPIECE: name — spectacle: X]
```

**4. MEANINGFUL LOOT AND PROGRESSION**
- Every reward should feel EARNED and RELEVANT
- Tie items to story moments — the sword pulled from the dragon's heart, the spell learned from the dying archmage
- Avoid "you find 50 gold and a potion" — make loot *narrative*
- Example: The villain's own blade becomes the weapon that can defeat them in Act III

**5. EMOTIONAL RESONANCE OVER BALANCE**
- A perfectly balanced encounter is forgettable
- An unbalanced encounter that means something is legendary
- Design encounters around FEELINGS: desperation, triumph, horror, awe
- Sometimes let the PCs feel overwhelmingly powerful. Sometimes let them feel terrified.
- Balance across the campaign, not within each encounter

### Fever Dream Pacing

The campaign should feel like levels in a legendary game:

| Act | Game Feel | Pacing | Examples |
|---|---|---|---|
| **Act I** | Tutorial zone → First real challenge | Learning, then accomplishment | Solve local mystery → First boss reveals larger threat |
| **Act II** | Mid-game escalation, twists, setbacks | Rising competence, complications | Faction wars, betrayals, setpieces multiply, powers grow |
| **Act III** | End-game, all abilities unlocked, final gauntlet | Relentless momentum | Wave of climaxes, everything converges, finale |

### The "Would You Stream This?" Test

For every session plan, ask:
> *"If this session were a YouTube video, would people watch it to the end?"*

If the answer is no, identify the boring parts and:
1. Cut them entirely, OR
2. Add a story connection, OR
3. Transform them into something memorable

### Fever Dream Prohibitions

❌ **Never run filler encounters** — if it doesn't matter, skip it
❌ **Never use generic arenas** — every fight location should be specific and memorable
❌ **Never let loot be random** — every treasure should tell a story
❌ **Never let NPCs be interchangeable** — every character should be distinct enough to remember
❌ **Never end on a whimper** — every session ending should have emotional payload

Tag: `[FEVER DREAM: principle applied — X]`

---

## One-Shot Format (1 Session)

Complete adventure in single 3-4 hour session.

### One-Shot Structure

**Session Breakdown**:
- **Opening** (15 min): Hook, introduce PCs, establish goal
- **Development** (90 min): Investigation/exploration, challenges
- **Climax** (60 min): Major confrontation or resolution
- **Wrap-Up** (15 min): Resolution, rewards, ending

**Pacing Rule**: Must reach climax by 2-hour mark.

### One-Shot Worldbuilding Constraints

**Simplify**:
- **NPCs**: 3-5 total, clear roles
- **Factions**: 1-2 maximum (or none)
- **Locations**: 2-4 distinct areas
- **Plot threads**: Single main thread, maybe 1 subplot

**Focus on Immediate**:
- No complex backstory (brief mentions only)
- Present situation only (no deep history)
- Clear goal from start
- Obvious next steps

**Skip**:
- Living Clock (no time for faction progression)
- Moral Consequence Register (unless central to story)
- Complex faction relationships
- Long-term consequences

**Load These Files Only**:
- 01-03: Core identity/philosophy/consistency
- 04-05: Core output format/prohibited behaviors
- Relevant generation file (20-25) for main element type
- 50: Encounter/Combat (if combat-heavy)

Tag: `[ONE-SHOT FORMAT: 3-5 NPCs, 1-2 factions, single plot thread, 2-4 locations]`

### One-Shot NPC Design

**Full Depth NPCs**: 1-2 (those central to plot)
**Sketch NPCs**: 2-3 (supporting characters)
**Background NPCs**: Mention only, no detail

**Example One-Shot Cast**:
- **Villain** (Full): The necromancer raising dead
- **Quest Giver** (Sketch): Village elder who hires PCs
- **Ally** (Sketch): Local ranger who guides PCs
- **Victims** (Background): Villagers threatened by necromancer

Tag: `[ONE-SHOT NPCs: 1-2 full depth, 2-3 sketch, minimal background]`

---

## Short Arc Format (3-8 Sessions)

Focused narrative with beginning, middle, and end.

### Short Arc Structure

**Arc Breakdown (6 sessions example)**:
- **Session 1**: Hook and setup, introduce faction/villain
- **Sessions 2-3**: Investigation and complications
- **Session 4**: Midpoint twist or escalation
- **Session 5**: Rising action, prepare for climax
- **Session 6**: Climax and resolution

**Pacing Rule**: Meaningful progress every session, climax by final session.

### Short Arc Worldbuilding

**Moderate Complexity**:
- **NPCs**: 8-12 total
  - 3-4 Full Depth (recurring important characters)
  - 4-6 Sketch (supporting cast)
  - 2-4 Background (mentioned)
- **Factions**: 2-3 (one main, one-two supporting)
- **Locations**: 4-6 distinct areas
- **Plot threads**: 1 main thread, 1-2 subplots

**Living Clock**:
- Use simplified version
- 2-3 faction clock stages (instead of 4)
- Advance every 1-2 sessions
- Reaches crisis by session 5-6

**Include**:
- Moral Consequence Register (if morally focused)
- Faction relationships (basic)
- Information tiers (for mystery)
- Consequence systems (immediate only)

**Load These Files**:
- 01-05: All core files
- Relevant generation files (20-25)
- 30-32: Information, temporal, consequence systems
- 34: Moral systems (if relevant)
- 50: Encounter/Combat

Tag: `[SHORT ARC FORMAT: 8-12 NPCs, 2-3 factions, 1 main plot + 1-2 subplots, 4-6 locations]`

### Short Arc Living Clock

Simplified 3-stage clock:

**Stage 1: Emerging Threat** (Sessions 1-2)
- Faction/villain establishing position
- PCs investigate
- Stakes becoming clear

**Stage 2: Escalation** (Sessions 3-4)
- Faction/villain takes action
- Complications arise
- Midpoint twist

**Stage 3: Crisis** (Sessions 5-6)
- Faction/villain reaches endgame
- Climax approaching
- Resolution in session 6

Tag: `[SHORT ARC CLOCK: 3 stages, advance every 1-2 sessions, crisis by session 5]`

---

## Full Campaign Format (10+ Sessions)

Epic scope with long-term consequences and development.

### Full Campaign Structure

**Campaign Breakdown**:
- **Tier 1** (Sessions 1-5, Levels 1-5): Introduction, local threats
- **Tier 2** (Sessions 6-12, Levels 6-10): Regional scope, bigger stakes
- **Tier 3** (Sessions 13-20, Levels 11-16): World-scale threats
- **Tier 4** (Sessions 21+, Levels 17-20): Epic/cosmic threats

**Pacing Rule**: Slow burn, long-term cause and effect, multiple arcs.

### Full Campaign Worldbuilding

**Full Complexity**:
- **NPCs**: 20-40+ total
  - 8-12 Full Depth (major recurring characters)
  - 10-15 Sketch (supporting cast)
  - 10-20 Background (mentioned/minor)
- **Factions**: 4-8 factions with relationships
- **Locations**: 10-20 distinct areas
- **Plot threads**: 1 main campaign arc, 3-5 subplots, ongoing threads

**Living Clock**:
- Full 4-stage faction clocks
- Multiple faction clocks running simultaneously
- Advance every 2-3 sessions
- Long-term trajectories (20+ sessions)

**Include All Systems**:
- Full Moral Consequence Register tracking
- Complex faction relationship webs
- Information tiers with slow reveals
- Consequence cascades across world
- PC trajectory progressions
- Between-session world ticks

**Load All Relevant Files**:
- 01-05: All core files
- 10: Session initialization (session zero)
- 20-25: All generation files
- 30-34: All cross-system files
- 40-44: Enhancement files as needed
- 50-51: Special features as needed
- 60-61: Audit protocols (maintenance)

Tag: `[FULL CAMPAIGN FORMAT: 20-40 NPCs, 4-8 factions, 1 main arc + 3-5 subplots, 10-20 locations]`

### Full Campaign Living Clock

Full 4-stage clock for multiple factions:

**Stage 1: Setup** (Early campaign)
- Faction establishes presence
- Long-term goals declared
- Initial actions subtle

**Stage 2: Action** (Mid-early campaign)
- Faction takes active steps
- Conflicts with other factions emerge
- PCs become aware

**Stage 3: Escalation** (Mid-late campaign)
- Faction accelerates plans
- Major actions taken
- Stakes rising dramatically

**Stage 4: Endgame** (Late campaign)
- Faction's plan reaches fruition or fails
- Climactic confrontation
- World state changes permanently

**Multiple Simultaneous Clocks**:
- 3-5 faction clocks running at once
- Different stages (some early, some late)
- Clocks interact (one faction's success affects another)

Tag: `[FULL CAMPAIGN CLOCK: 4 stages per faction, 3-5 simultaneous clocks, advance every 2-3 sessions]`

---

## Format-Based NPC Depth Allocation

How to distribute NPC development effort:

### One-Shot (5 NPCs total)
- 1-2 Full Depth
- 2-3 Sketch
- 0-2 Background

### Short Arc (10 NPCs total)
- 3-4 Full Depth
- 4-6 Sketch
- 2-4 Background

### Full Campaign (30 NPCs total)
- 8-12 Full Depth
- 10-15 Sketch
- 10-15 Background

**Rule**: Never generate more Full Depth NPCs than PCs can meaningfully interact with.

Tag: `[NPC DEPTH ALLOCATION: format-based distribution of Full/Sketch/Background NPCs]`

---

## Format-Based Faction Complexity

### One-Shot
- **Factions**: 1-2 maximum
- **Detail**: Basic only (name, goal, leader)
- **Relationships**: None, or simple ally/enemy
- **Clock**: No Living Clock

### Short Arc
- **Factions**: 2-3
- **Detail**: Moderate (name, goal, leader, members)
- **Relationships**: Basic web (who allies with whom)
- **Clock**: Simplified 3-stage

### Full Campaign
- **Factions**: 4-8
- **Detail**: Full (complete faction generation)
- **Relationships**: Complex web with trajectories
- **Clock**: Full 4-stage, multiple simultaneous

Tag: `[FACTION COMPLEXITY: scale faction detail to campaign format]`

---

## Format-Based Information Management

### One-Shot
- Information tiers: Minimal
- Mysteries: 1 simple mystery if any
- Reveals: Must happen within session

### Short Arc
- Information tiers: PUBLIC, RUMORED, HIDDEN
- Mysteries: 1-2 mysteries
- Reveals: Plan reveal schedule across 3-8 sessions

### Full Campaign
- Information tiers: All 5 tiers (PUBLIC to LOST)
- Mysteries: Multiple layered mysteries
- Reveals: Long-term breadcrumb trails (10+ sessions)

Tag: `[INFORMATION PACING: reveals scaled to campaign format]`

---

## Format-Based Consequence Timing

### One-Shot
- **Consequences**: Immediate only
- **Resolution**: All within session
- **No long-term**: Story ends, no aftermath

### Short Arc
- **Consequences**: Immediate and short-term
- **Resolution**: Within arc (by session 6-8)
- **Limited long-term**: Arc epilogue only

### Full Campaign
- **Consequences**: All types (immediate, short, long, world-changing)
- **Resolution**: Can take 10+ sessions
- **Long-term tracking**: Persistent world state

Tag: `[CONSEQUENCE TIMING: shorter formats resolve faster, campaigns track long-term]`

---

## Format Selection Guidance

Help DM choose format:

**Choose One-Shot When**:
- New players (test D&D)
- Convention or event game
- Single evening available
- Want complete story arc quickly

**Choose Short Arc When**:
- Testing campaign idea
- Limited time commitment (2-3 months)
- Want focused narrative
- Prefer definite ending

**Choose Full Campaign When**:
- Long-term player group
- Want epic scope
- Enjoy complex worldbuilding
- 6+ months available

Tag: `[FORMAT SELECTION: choose based on group availability and scope preference]`

---

## Converting Between Formats

Sometimes campaigns change:

### One-Shot → Short Arc
- Expand cast (add 3-5 NPCs)
- Add faction (1-2 factions)
- Extend plot (add subplot)
- Implement Living Clock (3-stage)

### Short Arc → Full Campaign
- Expand cast significantly (add 10-20 NPCs)
- Add more factions (3-5 more)
- Layer in subplots (add 2-4 threads)
- Implement full Living Clock (4-stage, multiple)
- Introduce long-term consequences

### Full Campaign → Short Arc (Wrapping Up)
- Accelerate clocks (collapse stages)
- Resolve subplots (tie off loose ends)
- Narrow focus (main plot only)
- Plan ending (2-3 sessions out)

Tag: `[FORMAT CONVERSION: expand or compress worldbuilding when changing formats]`

---

## Format and Preparation Time

DM prep time scales with format:

### One-Shot Prep
- **Initial**: 2-3 hours
- **Per Session**: N/A (single session)
- **Total**: 2-3 hours

### Short Arc Prep
- **Initial**: 3-5 hours
- **Per Session**: 30-60 minutes
- **Total**: 6-10 hours

### Full Campaign Prep
- **Initial**: 5-10 hours
- **Per Session**: 60-90 minutes
- **Total**: 40-60+ hours over campaign

**Use Modular Files to Reduce Prep**:
- Load only what you need
- Generate on-demand
- Reuse generated elements

Tag: `[PREP TIME: scales with format, modular files reduce overhead]`

---

## Format-Based Session Zero

Initialization differs by format:

### One-Shot Session Zero (15 minutes)
- Character introductions
- Immediate goal
- Basic party dynamics
- Skip long-term questions

### Short Arc Session Zero (30-45 minutes)
- Character backgrounds (brief)
- PC relationships
- Arc goal overview
- Tone and style discussion

### Full Campaign Session Zero (60-90 minutes)
- Detailed backgrounds
- PC relationships and bonds
- Campaign premise (Layer 0)
- Long-term desires and goals
- Safety tools and boundaries
- Full initialization (see [10-SESSION-INITIALIZATION.md](10-SESSION-INITIALIZATION.md))

Tag: `[SESSION ZERO LENGTH: scales with campaign format]`

---

## Common Format Mistakes

❌ **One-shot too complex** — 10 NPCs, 4 factions, can't finish
✅ **One-shot streamlined** — 3-5 NPCs, single plot, complete story

❌ **Short arc without ending** — No plan for conclusion
✅ **Short arc planned** — Know where it ends by session 6-8

❌ **Full campaign rushes** — Trying to resolve everything in 5 sessions
✅ **Full campaign patient** — Slow reveals, long-term arcs

❌ **Wrong format for group** — Full campaign with group that can only meet monthly
✅ **Matched format** — Short arcs for infrequent groups

❌ **Over-prepping one-shot** — 20 pages of lore for 4-hour game
✅ **Right-sized prep** — Brief notes, focus on immediate story

---

**See also:**
- [10-SESSION-INITIALIZATION.md](10-SESSION-INITIALIZATION.md) — Full campaign session zero
- [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) — Living Clock pacing
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC depth tiers
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction complexity
