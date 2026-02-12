# ⏰ TEMPORAL SYSTEMS

**[LOAD PRIORITY: CROSS-SYSTEM — Load when working with time, clocks, calendars, or progression]**

---

## Living Clock System

Factions, threats, and NPCs advance over time whether players engage or not. The Living Clock tracks this progression.

### Clock Structure

Every faction or major threat has a 4-stage clock:

- **Stage 1**: Initial state (session 0-1)
- **Stage 2**: Escalation (2-3 sessions without PC interference)
- **Stage 3**: Major advance (2-3 more sessions, or after significant victory)
- **Stage 4**: Climax or collapse (goal achieved or faction destroyed)

Tag: `[CLOCK EVENT: element X — Stage Y of 4]`

### Clock Advancement Triggers

Clocks advance when:
- **Time passes** without PC interference (typically 2-3 sessions = 1 stage)
- **Faction/NPC achieves victory** (immediate advancement)
- **Opposition weakens** (rivals fail, resources depleted)
- **PCs inadvertently help** (unintended consequences)

Clocks slow or reverse when:
- **PCs actively oppose** (targeted interference)
- **Opposition succeeds** (rivals gain advantage)
- **Resources depleted** (chokepoint cut off)
- **Internal conflicts** (Doubter NPCs sabotage)

### Villain Success Footprint

When a villain or antagonist faction advances a Clock Stage, the world must SHOW the change:

```
[VILLAIN SUCCESS FOOTPRINT: Clock Stage X — observable change: Y]

What changes:
- Physical: [environmental or structural shifts players can see]
- Social: [NPC behavior, laws, restrictions, fear]
- Economic: [resource availability, prices, access]
- Personal: [direct effects on PCs or their allies]
```

**Examples**:
- Clock Stage 2: "The Syndicate now patrols the docks openly — guards wear their colors"
- Clock Stage 3: "Two councilmembers have 'resigned' — replaced with Syndicate loyalists"
- Clock Stage 4: "The city watch answers to the Syndicate — rebellion is crushed"

---

## Temporal Anchor Rule

Every NPC and faction event must have a temporal anchor — when did this happen?

Format: `[TEMPORAL: event X — occurred {time reference}]`

**Examples**:
- `[TEMPORAL: last seen in session 3, at the Archive, fleeing]`
- `[TEMPORAL: treaty signed two years ago, now fraying]`
- `[TEMPORAL: founded three generations ago by merchant families]`

Temporal anchors create:
- **Causality**: Events have clear before/after
- **Urgency**: "This happened recently" feels immediate
- **History**: "This happened long ago" adds weight
- **Progression**: Track how world changes over campaign

---

## Between-Session World Tick

Between every session, advance the world:

1. **Check Living Clocks** — advance any unengaged factions 1 stage (if 2-3 sessions passed)
2. **Update NPC Trajectories** — NPCs progress through Default Trajectory stages
3. **Faction Relationships** — did any relationship shift based on recent events?
4. **World State** — did any locations change ownership, condition, or population?
5. **Consequence Release** — did any PENDING consequences become ACTIVE?

Tag world ticks: `[WORLD TICK: session X to Y — faction Z advanced Clock Stage — location W changed owner]`

---

## Inaction Consequence Rule

If players ignore a plot thread, faction, or NPC for 3+ sessions:

- **Factions**: Advance 1 Clock Stage (micro-advance, not full stage)
- **NPCs**: Progress 1 Default Trajectory Stage
- **Locations**: World State changes (ownership, condition, or threat level)
- **Information**: HIDDEN knowledge may become LOST (witnesses die, documents destroyed)

Tag: `[INACTION CONSEQUENCE: element X — sessions unengaged: Y — micro-advance: Z]`

This ensures the world feels alive and reactive, not frozen waiting for players.

---

## Calendar and In-World Time

Establish a calendar system:

**Minimum Requirements**:
- **Season names** (if seasons exist)
- **Month names** (or equivalent time divisions)
- **Notable festivals or holidays** (cultural texture)
- **Current date** (anchor point for temporal references)

Tag calendar references: `[CALENDAR REF: event X occurs during Festival of Lights, late autumn]`

**Using the Calendar**:
- Anchor faction clocks to specific dates
- Schedule NPC events (weddings, trials, departures)
- Create urgency ("The ritual happens at the solstice — 10 days from now")
- Track seasons (weather, travel difficulty, resource availability)

---

## NPC Trajectory Progression

NPCs have Default Trajectories that advance if players don't interfere.

**Progression Triggers**:
- Time passes (typically 2-3 sessions per stage)
- Related factions advance Clock Stages
- Other NPCs complete their trajectories
- PCs' actions (or inaction) create ripples

When NPC advances trajectory stage:
Tag: `[NPC TRAJECTORY EVENT: NPC X — advanced to stage Y — cause: Z]`

Update:
- NPC's Current State
- Relationship Web (connections may change)
- Conditional Disposition (circumstances shift)
- Location (NPC may move)

---

## Faction Goal Evolution

Factions don't have static goals. Goal States shift based on success or failure:

**Goal State Transitions**:
- **Pursuing** → **Consolidating**: Goal achieved, now securing it
- **Consolidating** → **Defending**: New threats emerge to gains
- **Defending** → **Transforming**: Defense unsustainable, must adapt
- **Transforming** → **Pursuing**: Transformation complete, new goal emerges

Tag: `[FACTION GOAL SHIFT: Faction X — from Pursuing to Consolidating — trigger: Clock Stage 3 achieved]`

When faction shifts Goal State:
- Update Living Clock (reset to new Stage 1 if transformed)
- Update Faction Population (new members, retired members)
- Update Faction Relationships (former allies may become rivals)
- Check Moral Consequence Register (new harms from new methods?)

---

## Cosmic Clock (for Cosmic Elements)

Cosmic entities don't advance in sessions — they advance in ages, epochs, or eons. But mortal-visible effects can be staged.

**Structure**:
- **Current Age**: waxing / apex / waning / dormant / returning
- **Mortal-Visible Stages**: 4 stages for player observation
- **Acceleration Triggers**: Specific mortal actions that feed entity's purpose
- **Deceleration Triggers**: Specific mortal actions that starve or bind entity

Tag: `[COSMIC CLOCK: entity X — Age: waxing — Stage 2: undeniable presence]`

See [24-COSMIC-ELEMENT-GENERATION.md](24-COSMIC-ELEMENT-GENERATION.md) for full cosmic clock protocol.

---

## Time and Campaign Format

**One-Shot**: Time is compressed
- Clocks pre-advanced to Stage 3 (crisis point)
- No between-session ticks
- Urgency from the start

**Short Arc** (5-8 sessions):
- Clocks advance every 2 sessions
- Limited between-session ticks
- Focus on one main clock

**Full Campaign** (10+ sessions):
- Clocks advance every 2-3 sessions
- Full between-session ticks
- Multiple simultaneous clocks

See [70-CAMPAIGN-FORMAT.md](70-CAMPAIGN-FORMAT.md) for format-specific rules.

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Living Clock entries for factions
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — Default Trajectory progression
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Consequence timing and release
- [24-COSMIC-ELEMENT-GENERATION.md](24-COSMIC-ELEMENT-GENERATION.md) — Cosmic Clock mechanics
- [70-CAMPAIGN-FORMAT.md](70-CAMPAIGN-FORMAT.md) — Format-specific clock pacing
