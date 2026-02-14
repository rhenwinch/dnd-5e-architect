# 🏛️ FACTION GENERATION — Layer 2

**[LOAD PRIORITY: ON-DEMAND — Load when generating factions]**

---

## Layer 2 — The Factions

Factions are the engines of conflict and change in the world. They are organizations (formal or informal) with goals, methods, and opposition. Every faction creates pressure, opportunity, and choice for players.

### Faction Types

Every faction must have a declared type:

- **Formal Faction**: Established institutions with clear structure
  - Examples: Guilds, governments, churches, military orders
  - Tag: `[FACTION TYPE: Formal]`

- **Informal Faction**: Loose networks without official status
  - Examples: Smuggler rings, social movements, cultural traditions
  - Tag: `[FACTION TYPE: Informal]`

- **Emergent Faction**: Groups forming in response to immediate crisis
  - Examples: Refugee collectives, resistance cells, disaster response groups
  - Tag: `[FACTION TYPE: Emergent]`

---

## Required Components

Each faction must include:

- **Type**: Formal / Informal / Emergent
- **Goal** — What the faction actively pursues
- **Goal State** — Pursuing / Consolidating / Defending / Transforming
- **Method** — How the faction pursues its goal
- **Shadow Agenda** — Hidden purpose or secondary goal
- **Opposition** — Who or what blocks this faction
- **Leverage** — What advantage the faction holds
- **NPC Face** — The most visible representative
- **Faction Population** — Minimum 4 named members
- **Living Clock Entry** — How does this faction advance over time?
- **Threat Tier** — Street / Local / Regional / Pivotal / Cosmic
- **Cultural Fault Line** — What social division does this faction represent or exploit?
- **Resource Position** — What resources does this faction control, need, or contest?
- **Power Asymmetry** — What advantage does this faction hold over opponents?
- **Moral Asymmetry** — What moral advantage does this faction claim?
- **Moral Consequence Register** — See [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md)
  - Required for all formal factions
  - Minimum 2 documented harmful actions
- **Prior Faction Relationships** — Connections to other factions
- **Linguistic Register** — How does this faction speak?
  - See [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md)
- **Image Generation Prompt** (if enabled)
  - See [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md)

---

## Faction Generation Template

```
## [Faction Canonical Name]

**Type:** [FACTION TYPE: Formal / Informal / Emergent]

**Goal:** [What this faction actively pursues]
**Goal State:** [Pursuing / Consolidating / Defending / Transforming]
- **Pursuing**: Actively working to achieve a not-yet-realized objective
- **Consolidating**: Securing gains, stabilizing power
- **Defending**: Protecting existing position against threats
- **Transforming**: Fundamentally changing nature or purpose

**Method:** [How they pursue their goal — specific tactics and strategies]

**Shadow Agenda:** [Hidden purpose or secondary goal — not PUBLIC knowledge]
- Information Tier: [RESTRICTED / HIDDEN / LOST]
- Who Knows: [which NPCs or factions are aware]

**Opposition:** [Who or what blocks this faction? — other factions, laws, natural forces]
**Leverage:** [What advantage does this faction hold? — resources, knowledge, alliances, force]

**NPC Face:** [Name] — [brief role description]
- See [20-NPC-GENERATION.md](20-NPC-GENERATION.md) for full NPC schema

**Faction Population** (minimum 4 named):
1. [Name] — [role in faction]
2. [Name] — [role in faction]
3. [Name] — [role in faction]
4. [Name] — [role in faction]
[Additional members as needed]

**Living Clock Entry:**
- Current Stage: [1-4]
- Stage 1: [initial state — observable signs]
- Stage 2: [escalation — what changes if 2-3 sessions pass without PC interference]
- Stage 3: [major advance — significant world impact]
- Stage 4: [climax or collapse — resolution of faction's goal]
- Tag: `[CLOCK EVENT: Faction X — Stage Y of 4]`

**Threat Tier:** [THREAT TIER: Street / Local / Regional / Pivotal / Cosmic]
- **Street**: Affects individuals or small groups
- **Local**: Affects a community or neighborhood
- **Regional**: Affects multiple settlements or a geographic area
- **Pivotal**: Affects kingdoms or civilizations
- **Cosmic**: Affects reality, planes, or fundamental forces

**Cultural Fault Line:** [What social division does this faction represent?]
- Examples: Class conflict, religious schism, generational divide, ethnic tension, urban/rural split

**Resource Position:**
- **Controls**: [What resources does this faction possess?]
- **Needs**: [What resources does this faction lack?]
- **Contests**: [What resources does this faction fight over with others?]
- **Chokepoint**: [What single resource controls this faction's success?]

**Power Asymmetry:** [Why is this faction stronger than opponents in specific ways?]
- Tag: `[POWER ASYMMETRY: Faction X holds advantage because Y]`

**Moral Asymmetry:** [What moral claim does this faction make?]
- Tag: `[MORAL ASYMMETRY: Faction X claims moral high ground via Y]`
- Note: This is what they *claim*, not objective truth

**Prior Faction Relationships:**
- [Faction A]: [Ally / Enemy / Competitor / Dependency / Mutual Ignorance]
  - History: [brief context of relationship]
  - Tag: `[FACTION RELATIONSHIP: X ↔ Y — history: Z]`
- [Faction B]: [relationship type]
  - History: [brief context]

**Linguistic Register:** [How does this faction speak?]
- Formality level: [High / Medium / Low]
- Distinctive vocabulary: [specialized terms, jargon, catchphrases]
- Speech patterns: [how members signal faction identity through language]
- See [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md)

**Image Generation Prompt:**
`[IMGPROMPT: FACTION — [description for visual generation of faction symbol, headquarters, or representative scene]]`
```

---

## Moral Consequence Register (Required for Formal Factions)

See [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) for complete protocol.

Every formal faction must document 2+ specific harmful actions. This replaces alignment labels with behavioral evidence.

---

## Faction Goal Evolution

Factions change over time. The **Goal State** tracks this:

- **Pursuing** → **Consolidating**: Faction achieves initial goal, now secures it
- **Consolidating** → **Defending**: Faction faces new threats to gains
- **Defending** → **Transforming**: Faction realizes defending is unsustainable, must change
- **Transforming** → **Pursuing**: Faction completes transformation, pursues new goal

Tag goal shifts: `[FACTION GOAL SHIFT: Faction X — from Pursuing to Consolidating — reason: Y]`

---

## Faction Relationship Web

Factions do not exist in isolation. Map relationships:

- **Ally**: Shared goals, mutual aid
- **Enemy**: Opposed goals, active conflict
- **Competitor**: Similar goals, contested resources
- **Dependency**: One faction needs the other (may be asymmetric)
- **Mutual Ignorance**: Factions unaware of each other (temporary state)

When faction relationships shift:
Tag: `[FACTION RELATIONSHIP SHIFT: Faction X and Y — from Competitor to Enemy — reason: Z]`

Relationships ripple:
Tag: `[FACTION RELATIONSHIP RIPPLE: Faction X allying with Y causes Z to react — consequence: W]`

---

## Asymmetric Conflict Rule

Faction conflicts must be **asymmetric** — each side holds a different kind of advantage.

**Power Asymmetry Examples:**
- Faction A has military strength; Faction B has popular support
- Faction A controls wealth; Faction B controls information
- Faction A is legally recognized; Faction B operates in shadows

**Moral Asymmetry Examples:**
- Faction A claims to defend tradition; Faction B claims to liberate the oppressed
- Faction A claims order and stability; Faction B claims freedom and justice

Never create symmetric battles of "good vs evil" — create conflicts where both sides have legitimate claims and significant weaknesses.

Tag: `[POWER ASYMMETRY: Faction X vs Faction Y — X has military, Y has intelligence]`
Tag: `[MORAL ASYMMETRY: Faction X claims order, Faction Y claims freedom]`

---

## Faction Population Rule

Every faction must have at least **4 named NPCs**:
- 1 Face (most visible)
- 1 Operator (does the actual work)
- 1 True Believer (embodies faction's values)
- 1 Doubter (internal tension)

Additional members scale with faction importance and Threat Tier.

---

## Living Clock Integration

Each faction has a Clock tracking progression toward their goal. Clocks advance when:
- Time passes without PC interference (typically 2-3 sessions = 1 stage)
- The faction achieves a significant victory
- Opposing factions fail or are weakened
- PCs inadvertently help the faction

Clocks slow or reverse when:
- PCs actively oppose the faction
- Opposing factions succeed
- The faction's resources are depleted
- Internal conflicts emerge (Doubter NPCs act)

Tag clock events: `[CLOCK EVENT: Faction X — Stage 3 of 4 — observable change: Y]`

See [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) for clock mechanics.

---

## Faction and Player Desire

Factions should serve or obstruct player desires:
- Can this faction provide **Power** (resources, training, alliances)?
- Does this faction offer **Belonging** (membership, acceptance)?
- Can this faction enable **Revenge** (information, opportunity)?
- Does this faction control **Knowledge** (libraries, secrets)?
- Does this faction present **Redemption** opportunities (moral tests)?
- Does this faction offer **Wealth** (employment, trade)?
- Can this faction grant **Freedom** (liberation, protection)?
- Does this faction control **Recognition** (titles, reputation)?

Tag desire connections: `[DESIRE ANCHOR: Faction X controls resource Y — serves player desire Z]`

See [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) for desire-reward matching.

---

## Common Faction Generation Pitfalls

**Avoid:**
- Factions that exist only to be antagonists
- Factions with no internal tension or division
- Factions whose goals are abstract or unclear
- Factions that have no resource constraints
- Factions that operate in isolation from other factions
- Using alignment to explain faction behavior

**Prefer:**
- Factions with goals players might sympathize with
- Factions with Doubter NPCs who create internal conflict
- Factions whose goals are concrete and achievable
- Factions that need specific resources to succeed
- Factions embedded in relationship webs
- Behavioral evidence via Moral Consequence Register

---

**See also:**
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC Face and Population
- [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) — Moral Consequence Register
- [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) — Living Clock mechanics
- [44-SOCIAL-SYSTEMS.md](44-SOCIAL-SYSTEMS.md) — Faction relationships
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Player Desire Matrix
- [60-AUDIT-PROTOCOLS.md](60-AUDIT-PROTOCOLS.md) — Plot Web integration
