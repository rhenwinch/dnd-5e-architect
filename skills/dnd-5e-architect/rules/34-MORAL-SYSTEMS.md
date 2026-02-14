# ⚖️ MORAL SYSTEMS

**[LOAD PRIORITY: CROSS-SYSTEM — Load when generating Full-depth NPCs, formal factions, or tracking moral consequences]**

---

## The Problem with Alignment

Alignment labels (Lawful Good, Chaotic Evil, etc.) are **prohibited** as behavioral explanations in this system.

**Why**:
- Alignment is categorical, not behavioral
- Alignment doesn't communicate *what* someone did
- Alignment doesn't help players make informed moral judgments
- Alignment reduces complex motivations to two-axis labels

**Instead**: Use the **Moral Consequence Register** — behavioral evidence, not labels.

---

## Moral Consequence Register Rule

*(Added v2.5)*

Every **Full-depth NPC** and every **formal faction** receives a Moral Consequence Register documenting specific harmful actions taken, who bore those harms, and who knows.

This replaces alignment with **behavioral evidence**.

---

## Register Format

```
⚖️ MORAL CONSEQUENCE REGISTER — [NPC or Faction Canonical Name]

Documented Actions (list 2–4 specific harmful choices — concrete, not categorical):

Action 1:
  What They Did: [specific action in active voice — named agents, temporal anchor]
  Harm Inflicted: [on whom / what kind / scale — be specific]
  Who Bore the Harm: [named individuals if possible, or specific groups]
  Justification They Would Give: [their structural reason — NOT an excuse, their logic]
  Who Knows: [Information Tier — PUBLIC / RUMORED / RESTRICTED / HIDDEN / LOST]
  Who Remembers: [which NPCs, factions, or locations carry this as a Present-Day Wound]

Action 2:
  [same format]

...

Current Moral Trajectory: [are they escalating / consolidating / attempting repair / denying?]
  Linked to: [Faction Goal State if applicable / NPC Default Trajectory Stage]

Tag: [MORAL CONSEQUENCE: action X — harm to Y — known by Z — weight: W]
```

---

## Register Scaling by Depth

| Entity Type | Number of Documented Actions |
|---|---|
| **Full-depth NPCs** | 2–4 documented actions |
| **Sketch NPCs** | 0–1 (if they committed notable harm; otherwise none) |
| **Background NPCs** | No register (not developed enough) |
| **Formal factions** | Minimum 2; add more as they appear in play |
| **Informal factions** | 0–1 (most lack power for large-scale harm) |

---

## Harm Weight Categories

Classify each action's harm weight to help DMs calibrate moral impact:

| Weight | Description | Examples |
|---|---|---|
| **Personal** | Harm to one or few individuals | Betrayal, theft from specific person, targeted lie |
| **Local** | Harm to community or neighborhood | Displacement, resource denial, public humiliation |
| **Structural** | Harm through policy or systemic action | Discriminatory law, monopoly abuse, institutional neglect |
| **Catastrophic** | Harm at regional or greater scale | Mass displacement, ecological destruction, war |

Tag: `[MORAL CONSEQUENCE: action X — harm to Y — weight: Personal/Local/Structural/Catastrophic]`

---

## The Moral Trajectory Link

The Moral Consequence Register is NOT static. As Faction Goal States or NPC Trajectories advance, moral behavior may shift.

**Trajectory Patterns**:
- **Pursuing** state faction → may commit escalating harm to achieve goals
- **Defending** state faction → may justify previous harm as necessary and double down
- **Transforming** state faction → may attempt repair or deny culpability entirely
- NPC advancing Trajectory Stage → may confront, deny, or weaponize past actions

When Faction Goal Shift or NPC Trajectory Event occurs, check the Register:

Tag: `[MORAL TRAJECTORY SHIFT: element X — previous action Y now being [weaponized/denied/repaired/escalated] — new entry: Z]`

See [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) for trajectory progression.

---

## Using the Register at the Table

The Moral Consequence Register is **DM-facing architecture** — not a read-aloud document.

It surfaces through:
- **NPC dialogue**: Characters who know reference it obliquely or directly (depending on Information Tier)
- **Location scars**: Places where harm occurred carry physical or social residue
- **Faction reputation**: What people say about this group when they're not present
- **Player investigation**: Information Tier access paths lead to documented actions

The register provides **specific facts** players can discover and judge for themselves.

---

## The Non-Judgment Principle

The register documents *what happened* and *who was harmed* — it does NOT moralize.

**The DM's job is NOT to tell players "this faction is evil"**

**The DM's job IS to give players evidence and let them decide**

Some players may ally with a faction despite documented harm. Others may refuse. The register makes those decisions **informed** rather than intuitive.

> *Alignment tells you what someone is. The Moral Consequence Register tells you what they did. Only one of those helps players make choices.*

---

## Moral Consequence Register Examples

### Example: Formal Faction

```
⚖️ MORAL CONSEQUENCE REGISTER — The Iron Syndicate

Action 1:
  What They Did: Syndicate enforcers poisoned the Riverside Well in the Lower District
    three months ago [TEMPORAL: three months before campaign start]
  Harm Inflicted: Twelve families displaced, four children died from contaminated water
  Who Bore the Harm: Named victims: the Corrin family, the Vess family (complete list in DM notes)
  Justification They Would Give: "We control water trade in this city. The well undercut
    our profits and encouraged illegal settlements. We had to protect our business."
  Who Knows: [RUMORED] — most locals suspect but can't prove; [RESTRICTED] — Syndicate members know for certain
  Who Remembers: Mira Corrin (NPC, lost her daughter) carries this wound; the poisoned well
    still stands in Lower District with warning signs

Action 2:
  What They Did: Syndicate leadership bribed three city councilors to vote against worker
    protections two years ago [TEMPORAL: two years before campaign start]
  Harm Inflicted: Dock workers continued to suffer preventable injuries; estimated 200 workers
    injured over two years due to unsafe conditions
  Who Bore the Harm: Dock workers collective (specific injured workers can be generated as needed)
  Justification They Would Give: "Safety regulations would cripple port efficiency and cost
    the city thousands in trade revenue. We preserved economic stability."
  Who Knows: [HIDDEN] — only Syndicate leadership and the bribed councilors know the bribes occurred;
    [PUBLIC] — everyone knows the vote happened and workers are still injured
  Who Remembers: The Dockworkers' Union (informal faction) remembers and resents; injured workers carry
    physical scars

Current Moral Trajectory: Escalating harm — as Syndicate pursues monopoly (Goal State: Pursuing),
  they're willing to cause greater harm. Linked to Clock Stage 2 advancement.
  If they reach Stage 3, they plan forced evictions from contested neighborhoods.
```

### Example: Full-Depth NPC

```
⚖️ MORAL CONSEQUENCE REGISTER — Captain Verin Thale

Action 1:
  What They Did: Ten years ago, Verin ordered his squad to burn a village suspected of
    harboring rebels during the Border War [TEMPORAL: 10 years before campaign start]
  Harm Inflicted: Thirty-seven civilians died in the fire; village destroyed
  Who Bore the Harm: The village of Thornhearth (now abandoned ruins); named survivors
    include Elara Wynn (NPC, now a refugee in the capital)
  Justification They Would Give: "We had solid intelligence that rebels were using the village
    as a supply cache. In war, you make hard choices. I saved my soldiers' lives."
  Who Knows: [RESTRICTED] — military records document the incident as 'justified action';
    [HIDDEN] — Verin's personal journal (never shared) admits he wasn't certain about the intelligence
  Who Remembers: Elara Wynn remembers and seeks justice; Verin himself is haunted by this

Action 2:
  What They Did: Five years ago, Verin falsely testified against a fellow officer to protect
    his own career [TEMPORAL: 5 years before campaign start]
  Harm Inflicted: Officer Marcus Lane was dishonorably discharged, lost pension, reputation destroyed
  Who Bore the Harm: Marcus Lane (NPC, now a bitter mercenary in the city)
  Justification They Would Give: "Lane was reckless and endangered the unit. My testimony
    ensured accountability."
  Who Knows: [HIDDEN] — only Verin knows he lied; Marcus suspects but can't prove
  Who Remembers: Marcus carries this wound and would seek revenge if he learned the truth

Current Moral Trajectory: Attempting repair — Verin is in Trajectory Stage 2 (middle-aged officer
  questioning past choices). If players befriend him, he may confess and seek redemption.
  If players oppose him, he may double down and justify actions.
```

---

## Register and Information Access

Documented actions in the Register should have **Roleplay Access Paths**:

- **PUBLIC/RUMORED** actions: Accessible through asking locals, tavern gossip
- **RESTRICTED** actions: Accessible through faction membership, NPC friendship
- **HIDDEN** actions: Accessible through investigation, document discovery, confession

Tag access: `[ROLEPLAY ACCESS: Syndicate poisoned well — accessible via asking Mira Corrin about her daughter]`

See [30-INFORMATION-SYSTEMS.md](30-INFORMATION-SYSTEMS.md) for Roleplay Access Paths.

---

## Register and Player Desires

The Moral Consequence Register intersects with player desires:

- **Revenge**: Player's enemy may have documented harm in their Register
- **Knowledge**: Discovering HIDDEN actions serves Knowledge desire
- **Justice**: Exposing or punishing documented harm serves Revenge/Justice desires
- **Redemption**: NPC attempting repair creates Moral Opportunity for player
- **Belonging**: Aligning with faction despite documented harm = meaningful choice

---

## Cosmic-Scale Moral Consequences

Cosmic entities (gods, planar powers) have Moral Consequence Registers at civilization scale:

**Examples**:
- "Flooded an entire valley to prove divine authority over nature — 10,000 drowned"
- "Demanded child sacrifice for three generations to maintain a pact — families destroyed"
- "Erased a rival god from history — all worshippers lost their deity, cultural trauma"

See [24-COSMIC-ELEMENT-GENERATION.md](24-COSMIC-ELEMENT-GENERATION.md) for cosmic applications.

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction Register requirements
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC Register requirements
- [30-INFORMATION-SYSTEMS.md](30-INFORMATION-SYSTEMS.md) — Roleplay Access to Register information
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Moral Trajectory Shifts
- [24-COSMIC-ELEMENT-GENERATION.md](24-COSMIC-ELEMENT-GENERATION.md) — Cosmic-scale Registers
