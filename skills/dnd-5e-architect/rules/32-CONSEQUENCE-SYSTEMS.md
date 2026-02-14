# ⚖️ CONSEQUENCE SYSTEMS

**[LOAD PRIORITY: CROSS-SYSTEM — Load when tracking player actions, ripple effects, or consequences]**

---

## Consequence Triage Rule

Not all consequences should appear immediately. Triage them by urgency:

| State | Timing | When to Use |
|---|---|---|
| **PENDING** | Will surface in 2-3 sessions | Delayed ripples, long-term effects |
| **ACTIVE** | Currently affecting the world | Immediate consequences, ongoing effects |
| **RELEASED** | Already surfaced and resolved | Historical consequences now complete |

Tag format: `[CONSEQUENCE: PENDING/ACTIVE/RELEASED]`

---

## Consequence Web

Every significant player action should create ripples across multiple systems:

```
CONSEQUENCE WEB — [Player Action]

Immediate Effect:
- [What changes instantly in the location/situation]

Faction Reaction:
- [Which faction(s) respond, and how?]
- [Does this advance/slow any Living Clocks?]

NPC Reaction:
- [Which NPCs change disposition or trajectory?]
- [Do any NPCs remember this action?]

Location Impact:
- [Does World State change? — ownership, condition, population]
- [Does this affect other locations?]

Resource Shift:
- [Do any factions gain/lose resources?]
- [Does economic landscape change?]

Information Revelation:
- [What does this action reveal about the world?]
- [What HIDDEN knowledge becomes RUMORED or PUBLIC?]

Secondary Ripples:
- [What happens 2-3 sessions later if not addressed?]
- Tag: [CONSEQUENCE: PENDING — will surface in session X]

Tertiary Ripples:
- [What long-term effects if players never address this?]
- Tag: [CONSEQUENCE: PENDING — will surface in session Y if unresolved]
```

---

## Location Consequence Web

When players significantly change a location:

```
LOCATION CONSEQUENCE WEB — [Location Name] — [Player Action]

If players [specific action]:

→ Immediate Effect: [what changes in this location instantly]
→ Faction Reaction: [which faction(s) respond, and how]
→ NPC Reaction: [which NPCs change disposition or trajectory]
→ Secondary Location Impact: [does this affect other locations?]
→ Tag: [LOCATION CONSEQUENCE: action X in location Y causes faction Z to react with W]
```

**Examples**:
```
If players burn down the Archive:
→ Immediate Effect: All PUBLIC and RUMORED knowledge stored here becomes LOST
→ Faction Reaction: The Scribes become enemies; the Syndicate celebrates
→ NPC Reaction: Archivist Marin becomes hostile permanently
→ Secondary Location Impact: University loses access to historical records
→ Tag: [LOCATION CONSEQUENCE: burning Archive — Scribes become enemies]
```

---

## Inaction Consequence

The world progresses whether players act or not.

**Tracking Inaction**:
For each major faction, NPC, or plot thread:
- Count sessions since players last engaged
- At 3 sessions: Minor advance (micro-progress toward goal)
- At 5 sessions: Moderate advance (full Clock/Trajectory stage)
- At 7+ sessions: Major advance (cascade effects, may become irreversible)

Tag: `[INACTION CONSEQUENCE: element X — sessions unengaged: Y — advance: Z]`

**Examples**:
- `[INACTION CONSEQUENCE: The Syndicate — sessions unengaged: 4 — advance: Clock Stage 2→3, now controls docks]`
- `[INACTION CONSEQUENCE: NPC Marin — sessions unengaged: 3 — advance: Trajectory Stage 1→2, now desperate]`

---

## Reward Echo Rule

When players receive a reward, third parties OBSERVE and REACT:

```
REWARD ECHO — [Reward Type] — [Source]

Reward Received: [what the player got]
Observable Change: [what others can see about the player now]

Third-Party Reactions:
- Faction A: [how do they react? — respect, fear, jealousy, challenge]
- NPC B: [how do they react? — approach player, avoid player, request help]
- Faction C: [how do they react? — opportunity or threat?]

Future Consequence: [what happens 1-2 sessions later because player has this reward?]
Tag: [REWARD ECHO: reward type X — third party Y reacts with Z — future consequence: W]
```

**Reward Type Reactions** (from [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md)):
- **Capability rewards** → someone notices PC has new power and reacts
- **Relationship rewards** → third parties notice new alliance
- **Justice rewards** → defeated party's allies react
- **Information rewards** → source knows PC knows
- **Moral Opportunity rewards** → reputation shift
- **Material rewards** → economic position shifts
- **Constraint Removal rewards** → former authority loses leverage
- **Status rewards** → reputation spreads, opportunities and dangers

---

## Moral Trajectory Shift

When a Faction Goal State or NPC Trajectory advances, check the **Moral Consequence Register**:

Does the faction/NPC:
- **Escalate harm** (new entry in Register)
- **Consolidate previous harm** (double down, justify)
- **Attempt repair** (acknowledge, make amends)
- **Deny culpability** (reframe, lie)

Tag: `[MORAL TRAJECTORY SHIFT: element X — previous action Y now being [escalated/consolidated/repaired/denied] — new entry: Z]`

See [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) for Moral Consequence Register details.

---

## Villain Success Footprint

When antagonists advance Living Clock stages, the world must SHOW the change.

Observable effects when villain Clock advances:

**Physical Mark**:
- Environmental changes players can see
- New structures, destroyed buildings
- Territory expansion, border shifts

**Social Mark**:
- NPC behavior changes
- New laws or restrictions
- Fear, compliance, or resistance

**Economic Mark**:
- Resource availability shifts
- Prices change, trade disrupted
- New monopolies or chokepoints

**Personal Mark**:
- Direct effects on PCs or their allies
- Named NPCs harmed or changed
- Player-owned properties affected

Tag: `[VILLAIN SUCCESS FOOTPRINT: Clock Stage X — change category: Y — observable: Z]`

---

## Cascade Tracking

Some consequences trigger other consequences. Track cascades:

```
CASCADE — [Initial Action]

Primary Consequence: [first-order effect]
  ↓
Secondary Consequence: [effect caused by Primary]
  ↓
Tertiary Consequence: [effect caused by Secondary]
  ↓
Stabilization Point: [where does the cascade stop?]
```

**Example**:
```
CASCADE — Players destroy Syndicate warehouse

Primary: Syndicate loses shipment of weapons
  ↓
Secondary: Rival gang (the Crows) sees weakness, attacks Syndicate territory
  ↓
Tertiary: Gang war erupts in the docks, civilians flee
  ↓
Stabilization: City guard intervenes, imposes martial law
```

---

## World State Updates

When major consequences resolve, update World State:

Tag: `[WORLD STATE UPDATE: element X — previous: Y — current: Z — cause: W]`

**What to track**:
- Location ownership or control
- Faction power levels and relationships
- NPC disposition or trajectory stage
- Resource availability or scarcity
- Information tier shifts (HIDDEN becomes PUBLIC after reveal)

**Examples**:
- `[WORLD STATE UPDATE: The Archive — previous: neutral ground — current: controlled by Syndicate — cause: Clock Stage 3]`
- `[WORLD STATE UPDATE: NPC Marin — previous: neutral — current: hostile — cause: PC burned Archive]`
- `[WORLD STATE UPDATE: Iron supply — previous: contested — current: monopolized by Syndicate — cause: warehouse raid failed]`

---

## Consequence and Player Desire

Consequences should intersect with player desires:

- Consequence threatens what player values → creates urgency
- Consequence rewards what player desires → creates satisfaction
- Consequence shifts what player can access → creates new strategy

Tag desire intersections: `[CONSEQUENCE: action X — affects player desire Y via Z]`

See [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) for Player Desire Matrix.

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction reactions and Clock advancement
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC disposition shifts and trajectory
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Location Consequence Web
- [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) — Inaction and time-based consequences
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Reward Echo
- [34-MORAL-SYSTEMS.md](34-MORAL-SYSTEMS.md) — Moral Trajectory Shifts
