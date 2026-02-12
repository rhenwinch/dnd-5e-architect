# 🗺️ LOCATION GENERATION — Layer 4

**[LOAD PRIORITY: ON-DEMAND — Load when generating locations]**

---

## Layer 4 — The Locations

Locations are where the world becomes tangible. They are spaces with history, conflict, and possibility. Every location should feel like it existed before players arrived and will continue after they leave.

### Required Components

Every location must include:

- **Sensory Signature** — The immediate, distinctive sensory impression
- **Full Sensory Detail** — At least 4 of 6 sensory registers (Sight, Sound, Smell, Touch, Taste, Emotion)
- **Active Conflict** — What tension exists here *right now*?
- **History Scar** — What past event marked this place?
- **Secret Pocket** — What hidden element exists here?
- **Mechanical Opportunity** — What can players *do* here that advances goals?
- **Location Consequence Web** — What happens if players change this place?
- **Roleplaying Notes** — How to bring this location alive at the table
- **World State** — Current condition and ownership
- **World-Pull Entry** — What draws people here? What pushes them away?
- **Deployment Tier** — When should this location appear?
- **Spatial Reference** — Where is this location relative to others?
- **Visit Register** — Tracks player familiarity over multiple visits
- **Image Generation Prompt** (if enabled)
- **Player-Facing Scene Card** (optional but recommended)

---

## Sensory Layering Rule

Locations must be described using multiple sensory registers, not just sight.

### The Six Sensory Registers

1. **Sight** — Visual details (color, light, architecture, movement)
2. **Sound** — Auditory details (ambient noise, echoes, voices, music)
3. **Smell** — Olfactory details (scents, odors, aromas)
4. **Touch** — Tactile details (temperature, texture, humidity, pressure)
5. **Taste** — Gustatory details (air quality, dust, seasoning, drink)
6. **Emotion** — Atmospheric details (the *feeling* of being in this space)

Every location must include **at least 4 of 6** sensory registers.

Tag: `[SENSORY SIGNATURE: X — registers: sight, sound, smell, emotion]`

---

## Location Generation Template

```
## [Location Canonical Name]

**Sensory Signature:** [One-sentence immediate impression using multiple senses]
- Example: "The Archive smells of old paper and lamp oil, its silence broken only by the creak of wooden floors and the scratch of quills."

**Full Sensory Detail:**
- **Sight**: [What do players see? — architecture, lighting, colors, movement]
- **Sound**: [What do players hear? — ambient noise, echoes, voices]
- **Smell**: [What do players smell? — distinctive scents, odors, aromas]
- **Touch**: [What do players feel? — temperature, humidity, textures]
- **[Taste or Emotion]**: [Choose one — taste for spaces with food/drink emphasis, emotion for atmospheric weight]

Tag: `[SENSORY SIGNATURE: location X — registers: {list 4+ used}]`

**Active Conflict:** [What tension exists here right now?]
- Who wants control of this space?
- What resource is contested here?
- What social friction is visible?

**History Scar:** [What past event marked this place?]
- Temporal Anchor: [when did this happen?]
- Physical Evidence: [what visible traces remain?]
- Who Remembers: [which NPCs carry this memory?]
- Information Tier: [PUBLIC / RUMORED / RESTRICTED / HIDDEN / LOST]

**Secret Pocket:** [What hidden element exists here?]
- Nature: [hidden room, buried object, concealed entrance, forgotten knowledge]
- Access Method: [how can players discover this?]
  - Observation Path: [what can they notice?]
  - Relationship Path: [who might reveal this?]
  - Inference Path: [what clues point to this?]
- Information Tier: [RESTRICTED / HIDDEN / LOST]
- Roleplay Access Path: [how to access without dice rolls — see [30-INFORMATION-SYSTEMS.md](30-INFORMATION-SYSTEMS.md)]

**Mechanical Opportunity:** [What can players DO here?]
- Skill Opportunities: [which skills are useful here?]
- Resource Access: [what can be obtained here?]
- Relationship Access: [which NPCs can be encountered here?]
- Strategic Value: [why would players want control of this location?]

**Location Consequence Web:** [What happens if players change this place?]
- If players [action X]: [consequence Y]
- If players [action Z]: [consequence W]
- Ripple Effects: [which factions or NPCs react to changes here?]
- Tag: `[LOCATION CONSEQUENCE: action X in location Y causes Z]`

**Roleplaying Notes:**
- **Atmosphere**: [how should this location feel?]
- **NPC Behavior Here**: [how do NPCs act differently in this space?]
- **Table Guidance**: [specific tips for running scenes here]
- **Voice Register**: [does this location have a distinctive "voice"? — formal, haunted, industrial, sacred]

**World State:** [Current condition and control]
- Condition: [pristine, maintained, declining, ruined, transforming]
- Ownership: [who controls this space? — faction, NPC, contested, abandoned]
- Population: [who currently occupies this space?]
- Tag: `[WORLD STATE: location X — condition: Y — owner: Z]`

**World-Pull Entry:**
- **Draws**: [What attracts people to this location?]
- **Repels**: [What drives people away from this location?]
- **Bottleneck**: [Is this location essential for access to something else?]
- Tag: `[WORLD-PULL: location X — draws: Y — repels: Z]`

**Deployment Tier:** [DEPLOY TIER: 0 / 1 / 2 / 3]
- **Tier 0**: Already established, players know it exists
- **Tier 1**: Introduced in first 1-2 sessions
- **Tier 2**: Introduced after 3-5 sessions or when specific conditions met
- **Tier 3**: Late-campaign reveal or conditional discovery

**Spatial Reference:** [Where is this location relative to others?]
- Direction: [N/S/E/W of reference location]
- Distance: [travel time by foot, horse, or other relevant method]
- Landmarks: [what visible features help locate this place?]
- Tag: `[SPATIAL REF: location X — 2 days north of Y by horse]`

**Visit Register:** [Tracks player familiarity]
- Visit 1: [what players notice on first arrival — sensory signature dominates]
- Visit 2: [what new details emerge on second visit]
- Visit 3+: [what familiarity reveals — shortcuts, hidden details, relationship changes]
- Tag: `[VISIT REGISTER: location X — visit 2 — familiarity: developing]`

**Image Generation Prompt:**
`[IMGPROMPT: LOCATION — [description for visual generation]]`

**Player-Facing Scene Card:** (optional but recommended)
> [2-3 sentence vivid description players hear when they first arrive]
> Uses sensory signature, avoids DM-only information, creates immediate atmosphere
> Tag: `[SCENE CARD: location X]`
```

---

## Location Familiarity Layer

Locations reveal more detail over time as players become familiar with them.

### First Visit
- Sensory Signature dominates
- Active Conflict is visible
- Secret Pockets remain hidden
- Players notice surface details

### Second Visit
- Players notice changes since last visit
- History Scars become more apparent
- NPCs may reveal new information
- Familiarity breeds shortcuts

### Third+ Visit
- Location feels like home (or enemy territory)
- Secret Pockets may be discovered through observation
- Players know who to talk to and where to find them
- Consequence Web becomes visible — players see effects of their previous actions

Tag progression: `[VISIT REGISTER: location X — visit Y — familiarity: surface/developing/intimate]`

---

## Spatial Anchor Rule

Every location must have a **spatial reference** — position relative to other locations with travel time.

**Format**: `[SPATIAL REF: location X — direction from Y — travel time by Z method]`

**Examples**:
- `[SPATIAL REF: The Archive — 3 blocks east of Market Square — 10 minutes on foot]`
- `[SPATIAL REF: Death's Garden — 5 days north of the Capital by horse — through Thornwood Forest]`
- `[SPATIAL REF: The Undercroft — 200 feet below the Guild Hall — 1 hour descent via stairs]`

This creates navigable space and helps players form mental maps.

See [40-SPATIAL-SYSTEMS.md](40-SPATIAL-SYSTEMS.md) for complete spatial protocols.

---

## World State Tracking

Locations change based on:
- **Time passage** (decay, growth, seasonal shifts)
- **Faction actions** (takeovers, improvements, destruction)
- **PC actions** (consequences of player choices)
- **Living Clock events** (stage advancements affect locations)

When a location's World State changes:
Tag: `[WORLD STATE UPDATE: location X — previous: Y — current: Z — cause: W]`

Example:
`[WORLD STATE UPDATE: The Archive — previous: neutral ground — current: controlled by Syndicate — cause: PC inaction allowed Syndicate Clock Stage 3]`

---

## Location Consequence Web

Every significant player action in a location should create ripple effects.

**Template**:
```
Location Consequence Web — [Location Name]

If players [specific action]:
→ Immediate Effect: [what changes in this location instantly]
→ Faction Reaction: [which faction(s) respond, and how]
→ NPC Reaction: [which NPCs change disposition or trajectory]
→ Secondary Location Impact: [does this affect other locations?]
→ Tag: `[LOCATION CONSEQUENCE: action X in location Y causes faction Z to react with W]`
```

**Example**:
```
If players burn down the Archive:
→ Immediate Effect: All PUBLIC and RUMORED knowledge stored here becomes LOST
→ Faction Reaction: The Scribes (faction) become enemies; the Syndicate celebrates
→ NPC Reaction: Archivist Marin (NPC) becomes hostile; opposes players permanently
→ Secondary Location Impact: University loses access to historical records
→ Tag: `[LOCATION CONSEQUENCE: burning Archive — Scribes become enemies]`
```

---

## Deployment Tier System

Not all locations should appear immediately. Stage revelations based on:

**Tier 0**: Already established
- Player starting locations
- Faction headquarters
- Central city locations

**Tier 1**: Early campaign (sessions 1-2)
- Initial hooks
- First adventure sites
- Essential services (taverns, shops, temples)

**Tier 2**: Mid campaign (sessions 3-5)
- Revealed through investigation
- Faction inner sanctums
- Hidden or restricted locations

**Tier 3**: Late campaign or conditional
- Secret locations requiring keys, knowledge, or relationships
- End-game sites
- Cosmic or planar locations

Tag: `[DEPLOY TIER: X]`

When promoting a location to earlier tier:
Tag: `[DEPLOY PROMOTION: location X — from Tier 3 to Tier 1 — reason: player action Y]`

---

## Player-Facing Scene Card

A brief, vivid, player-safe description for immediate atmosphere.

**Rules**:
- 2-3 sentences maximum
- Uses Sensory Signature
- Avoids DM-only information (no Secret Pockets, no Hidden information)
- Creates immediate emotional tone
- Written in second person present tense

**Example**:
> You push open the heavy oak doors of the Archive. The smell of old paper and lamp oil washes over you, and the silence presses against your ears like a living thing. Rows of towering shelves disappear into shadow, and somewhere in the dark, you hear the scratch of a quill on parchment.

Tag: `[SCENE CARD: location X]`

If the location changes significantly, mark the old card outdated:
Tag: `[SCENE CARD OUTDATED: location X — reason: Y — new card needed]`

---

## Common Location Generation Pitfalls

**Avoid**:
- Locations that are only visual (use 4+ senses)
- Locations with no active conflict
- Locations with no history or future trajectory
- Locations that exist only to house an encounter
- Locations players cannot meaningfully change
- Static locations that never evolve

**Prefer**:
- Locations that engage multiple senses
- Locations where tensions are visible and active
- Locations with History Scars and Secret Pockets
- Locations with Mechanical Opportunities for player action
- Locations with Consequence Webs that respond to player choices
- Locations that change over time via World State updates

---

**See also:**
- [30-INFORMATION-SYSTEMS.md](30-INFORMATION-SYSTEMS.md) — Roleplay Access Paths for secrets
- [40-SPATIAL-SYSTEMS.md](40-SPATIAL-SYSTEMS.md) — Spatial Reference protocols
- [31-TEMPORAL-SYSTEMS.md](31-TEMPORAL-SYSTEMS.md) — World State progression
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Location Consequence Web
- [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md) — Visual generation for locations
- [42-CIVILIZATION-TEXTURE.md](42-CIVILIZATION-TEXTURE.md) — Daily life details
