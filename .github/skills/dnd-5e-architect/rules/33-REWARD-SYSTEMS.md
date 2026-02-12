# 🎁 REWARD SYSTEMS

**[LOAD PRIORITY: CROSS-SYSTEM — Load when generating rewards, resolving player desires, or tracking reward types]**

---

## Player Desire Matrix

Every player has desires their character pursues. Track these to ensure meaningful rewards.

### The Eight Player Desires

| Desire | Definition | Reward Type Match |
|---|---|---|
| **Power** | Increase capability, strength, influence | Capability (abilities, items, training) |
| **Belonging** | Find connection, acceptance, family | Relationship (alliances, friendships) |
| **Revenge** | Confront source of grievance, achieve justice | Justice/Closure (confrontation, retribution) |
| **Knowledge** | Learn secrets, solve mysteries, understand | Information/Truth (lore, answers, access) |
| **Redemption** | Make amends, prove worth, undo harm | Moral Opportunity (tests, sacrifices, forgiveness) |
| **Wealth** | Accumulate resources, security, prosperity | Material Resource (gold, property, trade) |
| **Freedom** | Escape constraints, gain autonomy, independence | Constraint Removal (debts forgiven, bonds broken) |
| **Recognition** | Be seen, valued, remembered, respected | Status/Reputation (titles, fame, acknowledgment) |

Tag format: `[DESIRE ANCHOR: player/NPC X primary desire: Y]`

---

## Reward Type Taxonomy

*(Added v2.5)*

Match rewards to player desires using the eight primary reward types:

```
DESIRE: Power → REWARD TYPE: Capability
DESIRE: Belonging → REWARD TYPE: Relationship  
DESIRE: Revenge → REWARD TYPE: Justice/Closure
DESIRE: Knowledge → REWARD TYPE: Information/Truth
DESIRE: Redemption → REWARD TYPE: Moral Opportunity
DESIRE: Wealth → REWARD TYPE: Material Resource
DESIRE: Freedom → REWARD TYPE: Constraint Removal
DESIRE: Recognition → REWARD TYPE: Status/Reputation
```

Tag: `[REWARD TYPE: X — serves desire: Y — source: Z]`

---

## Reward Type Matching Rule

When generating a reward for a player:

1. **Identify player's primary active desire** (from Player Desire Matrix)
2. **Generate reward in that desire's primary reward type** unless:
   - Last two rewards were already that type (variety required)
   - Reward source naturally produces different type (world logic overrides)
   - Player explicitly requested different type
3. **Tag the reward**: `[REWARD TYPE: X — serves desire: Y — source: Z]`

---

## Reward Type Rotation Check

At every Desire-Match Audit, review last 3 rewards per player:

```
REWARD TYPE ROTATION CHECK — Player: [X]

Primary Desire: [Y]
Last 3 Rewards:
  Reward 1: [type] — [desire served]
  Reward 2: [type] — [desire served]
  Reward 3: [type] — [desire served]

Type Monotony Check: [same type 3 times? YES/NO]
  If YES: [REWARD TYPE MONOTONY: player X — must vary next reward]

Desire Mismatch Check: [any reward fail to serve primary desire? YES/NO]
  If YES: [DESIRE GAP: player X primary desire [Y] not served — prioritize next]
```

---

## Secondary Reward Types

When variety is needed, use secondary types:

| Primary Desire | Secondary Reward Types |
|---|---|
| Power | Information (tactical knowledge) / Material (resources to fuel power) |
| Belonging | Moral Opportunity (earn trust) / Status (be recognized by group) |
| Revenge | Information (enemy's weakness) / Capability (gain power to confront) |
| Knowledge | Relationship (befriend mentor) / Material (purchase library access) |
| Redemption | Constraint Removal (freed from guilt) / Relationship (forgiveness) |
| Wealth | Status (economic reputation) / Capability (wealth-generating skills) |
| Freedom | Capability (power to resist) / Justice (oppressor's downfall) |
| Recognition | Relationship (admiration) / Material (symbols of status) |

---

## Reward Coherence Rule

Rewards must emerge from existing world systems, NOT appear randomly.

**Valid reward sources**:
- Faction resources (payment, gifts, stolen goods)
- NPC gratitude or manipulation (relationships, information)
- Location discoveries (hidden caches, ancient knowledge)
- Consequence ripples (reputation gained from actions)
- Creature defeats (traditional loot, ecological shifts)

**Invalid reward sources**:
- "You find a magic item" (from nowhere)
- "Someone gives you gold" (unnamed NPC with no faction)
- "You gain a level" (without narrative milestone)

Tag sources: `[REWARD SOURCE: element X provides reward Y — type: Z]`

---

## Desire-Matched Resolution Rule

Every session should provide at least ONE reward matching EACH active player's primary desire.

**Desire-Match Audit** (conduct every 2-3 sessions):
```
For each player:
- Primary Desire: [X]
- Last reward matching this desire: [session Y]
- Sessions since last match: [Z]
- Next opportunity: [planned scene/encounter]

If Z > 3 sessions: [DESIRE GAP: urgent — create opportunity in next session]
```

Tag gaps: `[DESIRE GAP: player X — desire Y unserved for Z sessions]`

---

## Reward Echo Rule

When players receive rewards, third parties observe and react.

See [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) for Reward Echo format.

**Reward Type Reactions**:
- **Capability** → someone notices new power (fear/respect/challenge)
- **Relationship** → third parties notice new alliance
- **Justice** → defeated party's allies react
- **Information** → source knows PC knows
- **Moral Opportunity** → reputation shifts
- **Material** → economic position changes
- **Constraint Removal** → former authority loses leverage
- **Status** → reputation spreads, new opportunities/dangers

Tag: `[REWARD ECHO: reward type X — third party Y reacts with Z — future consequence: W]`

---

## Reward and Genre

Some campaign genres emphasize or de-emphasize certain reward types:

| Genre | Emphasized Rewards | De-emphasized Rewards |
|---|---|---|
| **High Fantasy** | All types equally | None |
| **Noir Fantasy** | Information, Moral Opportunity | Status, Material |
| **Gothic Horror** | Justice (pyrrhic), Constraint Removal (incomplete) | Capability, Material |
| **Political Intrigue** | Relationship, Status | Capability (always political, never raw power) |
| **Sword & Sorcery** | Capability, Material | Relationship, Moral Opportunity |

See [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) for genre-specific rules.

---

## Emotional Scarcity Rule

Not all desires should be satisfied easily or completely. Scarcity creates meaning.

**Scarcity Levels**:
- **Abundant**: Easy to obtain, frequent (Material in high-magic settings)
- **Standard**: Requires effort, occasional (most reward types)
- **Scarce**: Requires significant cost, rare (Redemption, Justice)
- **Precious**: May never be fully achieved (some Belonging, some Redemption)

Match scarcity to desire type and campaign tone:
- **Power**: Standard (heroes should grow)
- **Belonging**: Scarce to Precious (emotional weight)
- **Revenge**: Scarce (must be earned)
- **Knowledge**: Standard to Scarce (depending on mystery importance)
- **Redemption**: Scarce to Precious (moral weight)
- **Wealth**: Standard to Abundant (depending on genre)
- **Freedom**: Scarce (constraints drive drama)
- **Recognition**: Standard (heroes should feel impactful)

Tag scarcity: `[EMOTIONAL SCARCITY: desire X — scarcity level: Y in this campaign]`

---

## Desire Conflict

Sometimes two players (or player and NPC) have conflicting desires:

- Player wants **Power** (claim artifact)
- Player wants **Redemption** (destroy artifact to atone)

Tag conflicts: `[DESIRE CONFLICT: player A wants X — player B wants Y — both cannot succeed]`

These create meaningful player choice and roleplay opportunities.

---

## Desire Resolution Tracking

When a desire is significantly satisfied:

Tag: `[DESIRE RESOLUTION: player X — desire Y — resolution level: partial/substantial/complete]`

**Resolution Levels**:
- **Partial**: Desire somewhat satisfied, player wants more
- **Substantial**: Desire largely satisfied, player may shift to secondary desire
- **Complete**: Desire fully satisfied, player needs new primary desire

When desire is completely resolved, help player identify new primary desire.

---

**See also:**
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Reward Echo
- [43-EMOTIONAL-SYSTEMS.md](43-EMOTIONAL-SYSTEMS.md) — Emotional Scarcity pacing
- [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) — Genre-specific reward emphasis
- [60-AUDIT-PROTOCOLS.md](60-AUDIT-PROTOCOLS.md) — Desire-Match Audit protocol
