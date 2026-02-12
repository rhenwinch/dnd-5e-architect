# ⚡ COMPRESSION MODE — Quick Checklist

**[LOAD PRIORITY: CHECKPOINT — Condensed checklist for rapid generation and validation]**

---

## Purpose

This file provides **ultra-condensed checklists** for validating generations without loading full system files. Use when you need quick validation or when operating under severe token constraints.

**When to use:**
- Token budget is critical
- Need quick validation only (not full generation)
- Reviewing existing content for gaps
- Rapid prototyping

**When NOT to use:**
- Initial generation (load full files)
- Deep worldbuilding (need complete context)
- Complex multi-element requests

Tag: `[COMPRESSION MODE: condensed validation checklist, not for full generation]`

---

## File Organization Quick Reference

**CRITICAL:** See [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) for complete file organization rules.

### World Directory Structure

**ALL worlds must be organized under `worlds/` directory:**

```
worlds/
└── [world-name]/
    ├── [world-name]-readme.md          # World overview & quick reference
    ├── [world-name]-factions.md        # All factions and organizations
    ├── [world-name]-npcs.md            # All notable NPCs
    ├── [world-name]-monsters.md        # Creatures and bestiary
    ├── [world-name]-items.md           # Magic items and artifacts
    ├── [world-name]-regions.md         # Geographic regions
    ├── [world-name]-locations.md       # Specific locations and sites
    ├── [world-name]-timeline.md        # Historical events & Living Clock
    ├── [world-name]-cosmology.md       # Gods, planes, cosmic forces
    ├── [world-name]-spells.md          # Custom world spells
    └── campaigns/                      # Campaign subfolder
        └── [campaign-name]/
            ├── [campaign-name]-readme.md
            ├── [campaign-name]-pcs.md
            ├── [campaign-name]-session-log.md
            ├── [campaign-name]-plot-web.md
            └── [campaign-name]-canon.md
```

**Quick Rules:**
- World folder name: lowercase-with-hyphens (e.g., `shadow-crown-empire`)
- File names: `[world-name]-[type].md` (all lowercase)
- Campaigns go in: `worlds/[world-name]/campaigns/[campaign-name]/`
- Support existing worlds: Load from folder if user provides path

---

## Mode Detection Quick Reference

**CRITICAL:** See [02-CORE-WORLDBUILDING-PHILOSOPHY.md](02-CORE-WORLDBUILDING-PHILOSOPHY.md) and [10-SESSION-INITIALIZATION.md](10-SESSION-INITIALIZATION.md) for complete operational mode rules.

### Quick Mode Detection

**WORLD BUILDING MODE (Default):**
- User says: "Build a world", "Create a setting", "I need a region"
- No active players mentioned
- Output → `worlds/[world-name]/[world-name]-[type].md`
- Tag: `[MODE: World Building]`

**CAMPAIGN MODE:**
- User says: "My players", "Our session", "PC named X"
- Active campaign context present
- Output → World files + `worlds/[world-name]/campaigns/[campaign-name]/[campaign-name]-[type].md`
- Tag: `[MODE: Campaign — World: world-name]`

**If Uncertain:** Ask directly: *"Are you building a world or running a campaign?"*

---

## Structured Output Quick Reference

**CRITICAL:** See [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) for complete structured output requirements.

**Every .md file MUST include:**
- [ ] **Table of Contents** at top (with anchor links)
- [ ] **Clear section hierarchy** (##, ###, ####)
- [ ] **Cross-references** to related files (relative paths)
- [ ] **DM Secrets** separated from public info
- [ ] **Metadata header** (World name, date, format)

**Example Header:**
```markdown
# Shadow Crown Empire — Factions
**World:** shadow-crown-empire | **Updated:** 2026-02-12 | **Format:** World Building
```

---

## Ultra-Quick Validation Checklists

### ⚡ NPC Checklist (30 seconds)

- [ ] **Name** + pronunciation guide
- [ ] **Public role** (what world sees)
- [ ] **Private drive** (actual motivation)
- [ ] **Secret** (embargoed, DM only)
- [ ] **Speech pattern** (1-2 distinctive traits)
- [ ] **Trajectory** (where they're headed)
- [ ] **Relationships** (min. 2 other NPCs/factions)
- [ ] **Moral Consequence Register** (if Full Depth)
- [ ] **Tag system** used

### ⚡ Faction Checklist (30 seconds)

- [ ] **Name** + type (Formal/Informal/Emergent)
- [ ] **Public goal** + shadow agenda
- [ ] **Leader** + min. 4 named members
- [ ] **Power source** + opposition
- [ ] **Living Clock stage** (1-4)
- [ ] **Relationship web** (allied/enemy with who?)
- [ ] **Moral Consequence Register**
- [ ] **Tag system** used

### ⚡ Location Checklist (30 seconds)

- [ ] **Name** + spatial anchor (position relative to other locations)
- [ ] **Primary function** (what happens here)
- [ ] **Sensory details** (min. 4 of 6 registers)
- [ ] **Power structure** (who controls it)
- [ ] **Hidden element** (not obvious to visitors)
- [ ] **Connection points** (how to reach other locations)
- [ ] **Tag system** used

### ⚡ Region Checklist (30 seconds)

- [ ] **Name** + scale reference
- [ ] **Scarce resource** (drives conflict)
- [ ] **Primary factions** (min. 2)
- [ ] **Civilization texture** (daily life snapshot)
- [ ] **Linguistic profile** (how people talk)
- [ ] **Hidden truth** (what's really going on)
- [ ] **Player hooks** (3+ entry points)
- [ ] **Tag system** used

### ⚡ Creature Checklist (30 seconds)

- [ ] **Name** + CR appropriate to context
- [ ] **Ecological role** (what it does in world)
- [ ] **Resolution paths** (3 ways to resolve: Combat/Non-Combat/Unexpected)
- [ ] **Faction ties** (if any)
- [ ] **Distinctive features** (memorable traits)
- [ ] **Consequence if ignored** (what happens if PCs don't engage)
- [ ] **Tag system** used

### ⚡ Cosmic Entity Checklist (30 seconds)

- [ ] **Name** + titles (how known to mortals)
- [ ] **True nature** vs public belief
- [ ] **Mortal Instruments** (NPCs who serve)
- [ ] **Cosmic Clock** (long-term goals)
- [ ] **Contact protocol** (how mortals can reach)
- [ ] **World impact** (visible effects of existence)
- [ ] **Cosmic Moral Register** (if relevant)
- [ ] **Tag system** used

---

## World Building File Checklist

When creating world documentation:

### [world-name]-readme.md Must Include:

- [ ] **World Overview** (elevator pitch)
- [ ] **Core Premise** (Layer 0 format) — if campaign-specific, otherwise leave open
- [ ] **Genre and Tone** (explicit declaration)
- [ ] **Table of Contents** (links to all other world files)
- [ ] **Quick Reference** (key factions, regions, NPCs)
- [ ] **DM Secrets Section** (hidden truths separated)
- [ ] **Campaign Seeds** (3-5 potential campaign hooks)
- [ ] **Timeline** (major historical events)

### Each Content File Must Include:

- [ ] **Title** with world name
- [ ] **Table of Contents** (internal navigation)
- [ ] **Consistent Formatting** (headers, lists, tables)
- [ ] **Cross-References** (links to related files)
- [ ] **Tag System** (searchable tags throughout)
- [ ] **DM Notes** (separated from player-facing content)
- [ ] **Last Updated** (date stamp)

---

## Critical System Checks (1 minute)

### Consistency Check
- [ ] No contradictory facts
- [ ] NPCs know appropriate people
- [ ] Geography makes sense
- [ ] Timeline consistent
- [ ] Power levels appropriate

### Interconnection Check
- [ ] NPCs have relationships
- [ ] Factions interact
- [ ] Locations connected by travel
- [ ] Events have causes
- [ ] Consequences propagate

### Playability Check
- [ ] Clear hooks for players
- [ ] Multiple resolution paths
- [ ] Consequences for inaction
- [ ] Information accessible (not locked)
- [ ] Stakes clear and meaningful

### World vs Campaign Check
- [ ] **WORLD MODE:** Content stands alone, no PC assumptions
- [ ] **WORLD MODE:** Multiple campaigns could use this world
- [ ] **WORLD MODE:** NPCs exist independent of players
- [ ] **CAMPAIGN MODE:** PC integration points clear
- [ ] **CAMPAIGN MODE:** Session structure appropriate
- [ ] **CAMPAIGN MODE:** Player-specific tracking evident

---

## Rapid Generation Template

**For quick NPC:**
```
NAME (pronunciation) — PUBLIC ROLE
Private Drive: [motivation]
Secret: [EMBARGOED]
Speech: [pattern]
Knows: [2-3 NPCs]
Trajectory: [where heading]
[Tags]
```

**For quick Faction:**
```
FACTION NAME — [Type]
Goal: [public] / Shadow: [hidden]
Leader: [NPC] + Members: [4+ names]
Opposes: [who]
Clock: Stage [1-4]
[Tags]
```

**For quick Location:**
```
LOCATION NAME — [Region]
Function: [what happens here]
Senses: [4 registers]
Controlled by: [faction/NPC]
Hidden: [secret]
Access: [how to reach]
[Tags]
```

---

## File Organization Validation

### Before Finalizing World, Verify:

- [ ] All files in `worlds/[world-name]/` directory
- [ ] File naming convention followed (all lowercase)
- [ ] readme.md exists with overview
- [ ] Each file has Table of Contents
- [ ] Cross-references work (valid links)
- [ ] Tag system consistent across files
- [ ] DM secrets clearly separated
- [ ] No orphaned content (everything referenced)

### World Building Quality Markers:

- [ ] World can support multiple campaigns
- [ ] Content independent of specific PCs
- [ ] Factions have goals beyond player interaction
- [ ] NPCs have lives and relationships
- [ ] Time progresses naturally
- [ ] Geography and culture feel lived-in
- [ ] Hidden depths to discover
- [ ] Consequences exist without player trigger

---

## Token Budget Guidelines

**Minimum viable generation:**
- NPC (Sketch): ~200 tokens
- Faction (Basic): ~300 tokens
- Location (Simple): ~250 tokens

**Standard generation:**
- NPC (Full): ~800-1000 tokens
- Faction (Complete): ~1200-1500 tokens
- Location (Detailed): ~800-1000 tokens
- Region: ~1000-1200 tokens

**Comprehensive world:**
- Full region with 2 factions, 6 NPCs, 4 locations: ~8000-10000 tokens

---

## Emergency Compression

**If token budget critical, minimum required:**

1. **Name** (what is it called)
2. **Function** (what does it do)
3. **Conflict** (what tension exists)
4. **Hook** (why players care)
5. **Tag** (for reference)

Everything else can be expanded later through archaeology scan.

---

## Common Mistakes Quick-Check

- [ ] ❌ Generic fantasy tropes → ✅ Distinctive elements
- [ ] ❌ Isolated NPCs → ✅ Connected relationships
- [ ] ❌ Static world → ✅ Living Clock progression
- [ ] ❌ No consequences → ✅ Action ripples
- [ ] ❌ Everything max intensity → ✅ Emotional scarcity
- [ ] ❌ Plot-driven → ✅ Consequence-driven
- [ ] ❌ Perfect heroes/villains → ✅ Moral complexity
- [ ] ❌ Info-dump → ✅ Tiered information access
- [ ] ❌ Files scattered → ✅ Organized in world directory
- [ ] ❌ Campaign assumptions → ✅ World stands alone

---

## Mode Selection Quick Reference

**User Request** → **Mode** → **Key Differences**

"Build the Kingdom of Shadows" → WORLD BUILDING
- Create complete world documentation
- No PC assumptions
- Multiple campaign potential
- Output to `worlds/kingdom-of-shadows/`

"Start a campaign in the Kingdom of Shadows" → CAMPAIGN MODE
- Use or create world
- Add PC integration
- Session tracking
- Campaign-specific consequences

"Add an NPC to my world" → WORLD BUILDING
- NPC exists independently
- No player relationship assumed
- Part of world state

"Add an NPC for my players to meet" → CAMPAIGN MODE
- NPC designed for player interaction
- Session context assumed
- Campaign-specific role

---

## Compression Mode Limitations

**What Compression Mode CANNOT do:**
- Generate from scratch (needs full files)
- Handle complex multi-element requests
- Provide deep worldbuilding context
- Replace full audit protocols

**What Compression Mode CAN do:**
- Quick validation of existing content
- Rapid gap identification
- Emergency token-budget operation
- Checkpoint verification

**Always prefer full modular files for generation. Use compression only for validation.**

---

## Integration with Full System

**Compression Mode works WITH modular system:**

1. **Generate** using full modular files (CORE + relevant modules)
2. **Validate** using compression checklist
3. **Audit** using full audit protocols (60-61)
4. **Maintain** using archaeology (61) + audits (60)

**Compression is for speed, not depth.**

---

**See also:**
- [README.md](README.md) — Full modular loading guide
- [QUICK-START.md](QUICK-START.md) — 30-second system intro
- [60-AUDIT-PROTOCOLS.md](60-AUDIT-PROTOCOLS.md) — Comprehensive audit system
- [61-CANON-ARCHAEOLOGY.md](61-CANON-ARCHAEOLOGY.md) — World maintenance and consolidation
