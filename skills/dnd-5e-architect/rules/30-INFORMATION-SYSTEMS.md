# 📚 INFORMATION SYSTEMS

**[LOAD PRIORITY: CROSS-SYSTEM — Load when working with information tiers, knowledge distribution, or mysteries]**

---

## Information Tier System

All knowledge in the world exists at one of five tiers:

| Tier | Definition | Who Knows | Access Method |
|---|---|---|---|
| **PUBLIC** | Common knowledge available to anyone | Everyone | Ask any NPC |
| **RUMORED** | Widespread but unconfirmed information | Many, but reliability varies | Ask multiple sources, cross-reference |
| **RESTRICTED** | Limited to specific groups or individuals | Faction members, scholars, specialists | Relationship with insider, infiltration, research |
| **HIDDEN** | Actively concealed or protected | Very few NPCs, often antagonists | Investigation, interrogation, decryption |
| **LOST** | Forgotten, destroyed, or erased | Possibly no living person knows | Archaeological dig, magical vision, ancient text |

Tag format: `[PUBLIC]`, `[RUMORED]`, `[RESTRICTED]`, `[HIDDEN]`, `[LOST]`

---

## Information Access Design Rule

*(Added v2.5 — ensures knowledge is accessible through roleplay, not only dice rolls)*

Every piece of knowledge tagged as `[RESTRICTED]`, `[HIDDEN]`, or `[LOST]` must include at least one **Roleplay Access Path** — a way to obtain information through player engagement with the world that does NOT require a skill check.

Dice rolls remain available as **backup mechanism** — not primary path.

### Roleplay Access Path Format

```
🔍 ROLEPLAY ACCESS PATH — [Knowledge Description]

Information Tier: [RESTRICTED / HIDDEN / LOST]

Primary Access Path (dice roll — backup only):
  Skill: [Investigation / Insight / Perception / History / Arcana / Religion / Nature / etc.]
  DC: [appropriate to tier and importance]
  Success Reveals: [what the check uncovers]

Roleplay Access Path 1 (no dice required):
  Method: [Observation / Relationship / Behavior / Inference / Environmental]
  Trigger: [what the player must do or say in-character to access this knowledge]
  Example provided in generation

Tag: [ROLEPLAY ACCESS: knowledge X — accessible via Y]
```

### Roleplay Access Methods

| Method | Description | Example Triggers |
|---|---|---|
| **Observation** | Player describes examining something specific | "I look closely at the scar on his neck" / "I watch where she looks when she lies" |
| **Relationship** | Player invests in NPC relationship over time | Multiple conversations / sharing a meal / helping with personal problem |
| **Behavior** | Player acts in a way that naturally reveals information | Following someone / eavesdropping / participating in ritual |
| **Inference** | Player connects existing facts out loud | "If the guild controls the harbor and the Syndicate controls the foundry, that means..." — DM confirms or corrects |
| **Environmental** | Information physically present in the world | Written on wall / carved in tree / sung in tavern song |

### Tiering Roleplay Access Difficulty

| Information Tier | Roleplay Access Difficulty |
|---|---|
| **PUBLIC** | No Roleplay Access Path needed — anyone can ask anyone |
| **RUMORED** | Easy — asking the right person in the right place |
| **RESTRICTED** | Moderate — requires specific relationship, location, or observation |
| **HIDDEN** | Hard — requires multiple steps, trust-building, or clever inference |
| **LOST** | Very Hard — requires extensive investigation, multiple Roleplay Paths, or cosmic element contact |

---

## Distributed Knowledge Rule

No single source should hold all knowledge about a topic. Distribute information across:
- Multiple NPCs (each knows different pieces)
- Multiple locations (archives, ruins, art)
- Multiple factions (each has biased perspective)
- Multiple methods (observation, rumor, research)

**Minimum 2 access paths** for RESTRICTED knowledge
**Minimum 3 access paths** for HIDDEN knowledge

Tag: `[KNOWLEDGE PATH: Primary/Secondary/Tertiary — source: X — method: Y]`

---

## Mystery Preservation Rule

When generating mysteries:

**The Three Truths**:
1. **Surface Truth** — What players learn first (may be false)
2. **Deeper Truth** — What investigation reveals (partially true)
3. **Core Truth** — The actual reality (may never be fully revealed)

Each truth should:
- Be narratively satisfying if players stop there
- Create new questions when discovered
- Respect player agency (players aren't wrong for believing Surface Truth)

Tag revelations: `[REVELATION STAGE: mystery X — players discovered Deeper Truth]`

---

## Contested Knowledge

Some information has multiple "truths" depending on who you ask:

- Faction A believes X (serves their interests)
- Faction B believes Y (serves their interests)
- The actual truth is Z (which neither acknowledges)

This creates player choice: whose version do they trust?

Tag: `[CONTESTED KNOWLEDGE: topic X — Faction A claims Y — Faction B claims Z — actual: W]`

---

## Information and NPC Disposition

NPCs with Conditional Disposition have Information Tier access linked to their state:

- NPC currently `[CONDITIONAL OBSTACLE]` will NOT volunteer `[RESTRICTED]` information even if asked
- NPC currently `[CONDITIONAL ALLY]` will volunteer `[RESTRICTED]` information if relationship established
- NPC currently `[NEUTRAL]` will trade `[RESTRICTED]` information for favors, gold, or reciprocal information

Tag the link: `[ROLEPLAY ACCESS: knowledge X — accessible via NPC Y — requires disposition: ALLY or NEUTRAL]`

---

## Knowledge Bottleneck Warning

If HIDDEN or LOST information has only one access path and that path is:
- An NPC who can die
- A location that can be destroyed
- A faction that can be eliminated

Tag it as a bottleneck: `[KNOWLEDGE BOTTLENECK: information X — single source: Y — risk: Z]`

Then add backup access path or accept that information may become permanently inaccessible.

---

## DM Guidance for Information Access

When a player:
- Describes a specific action rather than calling for a skill check
- Asks an NPC a direct, specific question (not "can I roll Insight?")
- Investigates an object, location, or detail with stated method
- Connects two pieces of existing information out loud
- Invests genuine roleplay time in building an NPC relationship

→ Check if a Roleplay Access Path exists for any relevant knowledge. If yes, deliver the information. If no, offer the dice roll backup.

---

## Information and Reward Type

Information itself can be a reward. When used as reward:
- Must serve player desire (typically **Knowledge** desire, sometimes **Power** or **Revenge**)
- Must be actionable (players can do something with it)
- Must create new opportunities (not just lore dumps)

Tag: `[REWARD TYPE: Information — serves desire: Knowledge — creates opportunity: X]`

See [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) for reward typing.

---

> *Dice rolls tell you if your character succeeds. Roleplay tells you if your player is paying attention. Reward both, but make the second one feel better.*

---

**See also:**
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC Conditional Disposition and information access
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Secret Pockets and hidden information
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Information as reward type
- [60-AUDIT-PROTOCOLS.md](60-AUDIT-PROTOCOLS.md) — Knowledge Bottleneck checking
