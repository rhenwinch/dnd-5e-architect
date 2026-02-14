# 🎭 NPC GENERATION — Layer 3

**[LOAD PRIORITY: ON-DEMAND — Load when generating NPCs]**

---

## Layer 3 — The NPCs

NPCs are the human (or non-human) faces of factions, the sources of information, the agents of conflict, and the emotional anchors for players.

### Required Components

Every NPC must include:

- **Public Role** — What everyone knows this person does
- **Private Drive** — What this person actually wants (may differ from public role)
- **Secret** — `[BACKSTORY: EMBARGOED — DM only]`
  - What this person hides
  - Never reveal in initial generation
  - Surface gradually through play
- **Relationship Web** — Connections to other NPCs and factions
- **Player Interaction Axis** — How might players encounter/use this NPC?
- **Conditional Disposition** — How this NPC's attitude shifts based on player action
  - States: Ally / Neutral / Obstacle / Enemy /Conditional Ally / Conditional Obstacle
- **Default Trajectory** — What happens to this NPC if players don't interfere
  - Minimum 3 stages
  - Each stage shows progression or degradation
- **Roleplaying Notes** — Voice, mannerisms, speech patterns
  - Must include **Speech Register** (see [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md))
- **NPC Depth Tier** — Full / Sketch / Background
  - Determines how much detail to generate
  - Full-depth NPCs require Moral Consequence Register
- **Temporal Anchor** — When/where was this NPC last encountered?
- **PC Backstory Connection** (if applicable)
  - Only if player has volunteered a connection
  - Tag: `[PC BACKSTORY HOOK: X]`
- **Moral Consequence Register** (for Full-depth NPCs only)
  - See [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md)
  - Documents specific harmful actions taken
- **Last Encountered Beat** — What emotional state was this NPC in when last seen?
- **Image Generation Prompt** (if visual generation enabled)
  - See [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md)

---

## NPC Depth Tiers

### Full-Depth NPCs
- Faction leaders, recurring allies, major antagonists
- Complete schema required
- Moral Consequence Register required
- Default Trajectory with 3+ stages
- Speech Register fully developed
- Tag: `[NPC DEPTH: Full]`

### Sketch NPCs
- Supporting cast, faction members, plot-relevant characters
- Reduced schema: Public Role, Private Drive, one Secret
- Conditional Disposition optional
- Default Trajectory 2 stages
- Moral Consequence Register only if they've caused notable harm
- Tag: `[NPC DEPTH: Sketch]`

### Background NPCs
- Shopkeepers, guards, passersby
- Name, role, one distinctive trait
- No trajectory, no register
- Can be promoted to Sketch if players engage heavily
- Tag: `[NPC DEPTH: Background]`

---

## NPC Generation Template

```
## [NPC Canonical Name]

**Public Role:** [What everyone knows]
**Private Drive:** [What they actually want]
**Secret:** [BACKSTORY: EMBARGOED — DM only] — [Hidden truth]

**Relationship Web:**
- [NPC/Faction A]: [nature of connection]
- [NPC/Faction B]: [nature of connection]
- [NPC/Faction C]: [nature of connection]

**Player Interaction Axis:** [How players might encounter or use this NPC]
- Example: "Information broker for underworld contacts"
- Example: "Potential ally if players oppose the Syndicate"
- Example: "Obstacle to accessing the Archive"

**Conditional Disposition:**
- Default: [Ally / Neutral / Obstacle]
- If [player action X]: shifts to [new disposition]
- If [player action Y]: shifts to [new disposition]

**Default Trajectory** (if players do not interfere):
- Stage 1: [current state]
- Stage 2: [progression after 2-3 sessions]
- Stage 3: [final state if no intervention]
- Tag: `[NPC TRAJECTORY EVENT: stage X — change: Y]`

**Roleplaying Notes:**
- **Voice Register:** [Formal / Colloquial / Mythic / Predatory / Haunted / Technical]
  - See [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md)
- **Speech Register:** [specific patterns, vocabulary, cadence]
  - Example: "Speaks in clipped military phrases, never uses contractions"
  - Example: "Laughs nervously before revealing information"
- **Mannerisms:** [physical habits, tells, distinctive behaviors]
- **Emotional Range:** [what emotions does this NPC display? what do they hide?]

**Temporal Anchor:** [TEMPORAL: last seen in session X, location Y, emotional state Z]

**PC Backstory Connection:** (if applicable)
- [PC Name]: [nature of connection — only if player volunteered this]
- Tag: `[PC BACKSTORY HOOK: X]`

**Last Encountered Beat:** [Rising / Peak / Recovery] — [brief emotional summary]

**NPC Depth:** [Full / Sketch / Background]

**Image Generation Prompt:** (if enabled)
`[IMGPROMPT: NPC — [description for visual generation]]`
```

---

## Moral Consequence Register (Full-Depth NPCs Only)

See [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) for complete protocol.

Required for all Full-depth NPCs. Documents 2-4 specific harmful actions this NPC has taken, who was harmed, and who knows.

---

## NPC State Progression Rule

NPCs advance through their Default Trajectory stages based on:
- **Time passage** (Living Clock advancement)
- **Player inaction** (if players ignore this NPC for 3+ sessions, they advance one stage)
- **World events** (faction shifts, location changes, other NPC actions)

When an NPC advances a stage:
1. Update their Current State
2. Tag: `[NPC TRAJECTORY EVENT: NPC X — advanced to stage Y — reason: Z]`
3. Update Relationship Web if connections change
4. Update Conditional Disposition if circumstances shift
5. Check Moral Consequence Register — has this advancement caused new harm?

---

## NPC Consolidation Rule

When the NPC count exceeds manageable limits (typically 15+ named NPCs):
- Combine similar NPCs into single entities
- Retire NPCs who haven't appeared in 5+ sessions
- Promote Background NPCs to Sketch if players engage heavily
- Demote Sketch NPCs to Background if players never engage

Tag consolidations: `[NPC CONSOLIDATED: A + B → C — reason: X]`
Tag retirements: `[NPC RETIRED: X — reason: Y]`

See [61-CANON-ARCHAEOLOGY.md](61-CANON-ARCHAEOLOGY.md) for consolidation protocols.

---

## NPC and Player Desire

Every NPC should serve or obstruct at least one player desire. Check:
- Does this NPC help a player achieve **Power** (mentorship, training, magical items)?
- Does this NPC provide **Belonging** (friendship, acceptance, found family)?
- Does this NPC enable **Revenge** (information, assistance, confrontation opportunity)?
- Does this NPC offer **Knowledge** (secrets, lore, access to information)?
- Does this NPC present **Redemption** opportunities (forgiveness, moral tests)?
- Does this NPC control **Wealth** (resources, employment, trade)?
- Does this NPC affect **Freedom** (liberation, constraint removal, independence)?
- Does this NPC grant **Recognition** (public acknowledgment, titles, reputation)?

Tag desire connections: `[DESIRE ANCHOR: NPC X serves player desire Y]`

See [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) for desire-reward matching.

---

## Common NPC Generation Pitfalls

**Avoid:**
- NPCs who exist only to exposit or serve plot
- NPCs with no internal conflict or private drive
- NPCs whose disposition is static regardless of player action
- NPCs whose secrets are never discoverable
- NPCs who have no relationship to factions or other NPCs
- Using alignment to explain NPC behavior — use Moral Consequence Register instead

**Prefer:**
- NPCs who have goals that may conflict with players
- NPCs whose public role and private drive differ
- NPCs who change over time whether players engage or not
- NPCs whose secrets have multiple access paths
- NPCs who are embedded in faction and relationship webs
- Behavioral evidence over categorical labels

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction Population requirements
- [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) — Moral Consequence Register
- [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md) — Speech Registers
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Player Desire Matrix
- [61-CANON-ARCHAEOLOGY.md](61-CANON-ARCHAEOLOGY.md) — NPC Consolidation
- [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) — Temporal Anchors and progression
