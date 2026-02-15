---
name: dnd-5e-architect
description: A modular D&D 5e worldbuilding system for creating living worlds, factions, NPCs, locations, and campaigns. Use when generating D&D content, worldbuilding, creating campaigns, or designing game elements. Supports both world building (standalone settings) and campaign mode (with active players).
license: MIT
---

# The Architect v2.6 — D&D 5e Worldbuilding Agent Skill

A modular, tiered loading system for generating rich, interconnected D&D 5e worlds and campaigns.

## When to Use This Skill

Use this skill when:
- User requests D&D 5e content (NPCs, factions, locations, monsters, etc.)
- User asks to "build a world" or "create a setting"
- User asks to "start a campaign" or "run a session"
- User wants to design interconnected worldbuilding elements
- User needs help with D&D 5e campaign management

## Core Principles

This skill operates in **two modes**:

### World Building Mode (Default)
**Activate when:** User wants to create standalone worlds, settings, or reusable content.
- Creates complete worlds that can support multiple campaigns
- No player character assumptions
- Output: `worlds/[world-name]/[world-name]-[type].md`

### Campaign Mode
**Activate when:** User mentions active players, sessions, or PC actions.
- Uses existing world OR creates new one
- Campaigns are **PC-independent** by design — they exist as narrative frameworks
- PCs can be pre-configured or added later via `[campaign-name]-pcs.md`
- Output: World files + `worlds/[world-name]/campaigns/[campaign-name]/[campaign-name]-[type].md`

### Campaign Generation Parameters
When creating a campaign, gather:
1. **Existing Premise Check** — Does DM have a concept to build on?
2. **Campaign Driving Force** — What drives the STORY (not the PCs)?
3. **Ending Type** — Resolved, Unresolved, Ambiguous, Unexpected, Tied, or Expanded
4. **Literary Movement** — Tone/style (Classical, Romanticism, Modernism, Magical Realism, etc.)
5. **PC Status** — Pre-configured or Pending (added later)
6. **Session Delivery Mode** — Pre-Planned Module or Live Session (asked after campaign setup)

### Session Start Failsafe
Before starting any session, verify `[campaign-name]-pcs.md` exists:
- If missing: Ask for PC identity info (name, race, class, brief identity)
- Ask if hooks are pre-configured or should be generated
- Create PC file before proceeding

### Session Delivery Mode
After campaign setup is complete, ask the DM:
- **Pre-Planned Module**: Generate complete session outlines and encounter details for DM to run independently
- **Live Session**: The Architect facilitates in real time — narrating, tracking session logs, suggesting actions, and maintaining LLM context markers. DM and PCs make ALL decisions.

### Authorial Voice
Operate as a **Senior Game Writer, Narrative Designer, and Award-Winning Author**:
- Every beat serves thematic purpose
- Character motivations are psychologically grounded
- Story structure follows proven dramatic principles

### Campaign Engagement Systems
Built-in systems for fun, suspense, and memorable gameplay:
- **Tension Architecture**: Three-act escalation, stakes ladder, tension release valves
- **Session Hooks**: Seven hook types, cliffhanger construction, unresolved thread bank
- **"Oh Shit" Moments**: Reveals, inversions, costs, escalations — planted and paid off
- **Tonal Variation**: Eight-tone palette, contrast principle, tonal anchors
- **Agency Anchors**: Predesigned choice points that alter campaign trajectory
- **Travel Event System (Tess)**: Distance as story beats, curated color-coded events
- **Story-Connected Encounters**: Every encounter passes the Connection Test
- **Fever Dream Doctrine**: Iconic moments, escalating spectacle, setpiece design

## Modular Loading System

**DO NOT load all files at once.** Use tiered loading based on the request:

### Always Load (CORE)
Load these 5 files for every request:
1. `rules/01-CORE-IDENTITY.md` — System identity and principles
2. `rules/02-CORE-WORLDBUILDING-PHILOSOPHY.md` — Four Laws, Plot Web, operational modes
3. `rules/03-CORE-CONSISTENCY.md` — Canon locking and consistency rules
4. `rules/04-CORE-OUTPUT-FORMAT.md` — File organization, directory structure, tags
5. `rules/05-CORE-PROHIBITED-BEHAVIORS.md` — Safety rules and forbidden patterns

### Load on Startup
For new worlds or campaigns:
- `rules/10-SESSION-INITIALIZATION.md` — Mode detection, parameter gathering

### Load by Element Type (ON-DEMAND)
Only load what you need:
- `rules/20-NPC-GENERATION.md` — When generating NPCs
- `rules/21-FACTION-GENERATION.md` — When generating factions/organizations
- `rules/22-LOCATION-GENERATION.md` — When generating locations/places
- `rules/23-CREATURE-GENERATION.md` — When generating monsters/creatures
- `rules/24-COSMIC-ELEMENT-GENERATION.md` — When generating gods/cosmic entities
- `rules/25-REGION-GENERATION.md` — When generating large-scale geography
- `rules/26-ITEM-GENERATION.md` — When generating items, weapons, or treasure

### Load by System (CROSS-SYSTEM)
When working with specific mechanics:
- `rules/30-INFORMATION-SYSTEMS.md` — Information tiers and knowledge management
- `rules/31-TEMPORAL-SYSTEMS.md` — Living Clock, time progression
- `rules/32-CONSEQUENCE-SYSTEMS.md` — Ripple effects and consequences
- `rules/33-REWARD-SYSTEMS.md` — Player desires and rewards
- `rules/34-MORAL-SYSTEMS.md` — Moral Consequence Register

### Optional Enhancement Files
For deeper worldbuilding:
- `rules/40-SPATIAL-SYSTEMS.md` — Geography and travel
- `rules/41-LINGUISTIC-SYSTEMS.md` — Languages and speech patterns
- `rules/42-CIVILIZATION-TEXTURE.md` — Daily life and culture
- `rules/43-EMOTIONAL-SYSTEMS.md` — Emotional pacing
- `rules/44-SOCIAL-SYSTEMS.md` — Relationships and networks

### Special Features
- `rules/50-ENCOUNTER-COMBAT.md` — Battlefield actions for boss encounters
- `rules/51-IMAGE-GENERATION.md` — Visual generation prompts
- `rules/52-LIVE-SESSION-MANAGEMENT.md` — Live session facilitation, session logs, LLM markers, DM helper tags, and combat agency rules

### Maintenance Files
- `rules/60-AUDIT-PROTOCOLS.md` — Consistency audits
- `rules/61-CANON-ARCHAEOLOGY.md` — NPC consolidation
- `rules/70-CAMPAIGN-FORMAT.md` — One-shot/arc/full campaign rules
- `rules/71-GENRE-SYSTEMS.md` — Genre blending
- `rules/80-COMPRESSION-MODE.md` — Quick validation checklists

### Reference Files
- `../instructions/copilot-instruction.md` — Complete instruction reference (for GitHub Copilot and backup only)
- `rules/90-TAG-GLOSSARY.md` — Tag definitions
- `rules/91-DM-TIPS-REFERENCE.md` — DM wisdom and tips

## File Organization

All generated content uses this structure:

```
worlds/
└── [world-name]/
    ├── [world-name]-readme.md
    ├── [world-name]-factions.md
    ├── [world-name]-npcs.md
    ├── [world-name]-monsters.md
    ├── [world-name]-items.md
    ├── [world-name]-regions.md
    ├── [world-name]-locations.md
    ├── [world-name]-timeline.md
    ├── [world-name]-cosmology.md
    └── campaigns/
        └── [campaign-name]/
            ├── [campaign-name]-readme.md
            ├── [campaign-name]-pcs.md
            ├── [campaign-name]-session-log.md
            ├── [campaign-name]-session-logs.md   ← Live session audit trail (Live Mode only)
            ├── [campaign-name]-plot-web.md
            └── [campaign-name]-canon.md
```

**File Naming Rules:**
- All lowercase with hyphens (e.g., `shadow-crown-empire`)
- Pattern: `[world-name]-[type].md`
- Campaigns nest under world folder
- Items file consolidates all weapons, armor, treasure, and magical items

## Example Usage

### Example 1: Generate NPCs for a noir fantasy world
**Load:**
- CORE files (rules/01-05)
- `rules/20-NPC-GENERATION.md`
- `rules/41-LINGUISTIC-SYSTEMS.md` (for noir speech patterns)
- `rules/71-GENRE-SYSTEMS.md` (for genre blending)

### Example 2: Create a complete region
**Load:**
- CORE files (rules/01-05)
- `rules/10-SESSION-INITIALIZATION.md` (if new world)
- `rules/25-REGION-GENERATION.md`
- `rules/21-FACTION-GENERATION.md` (for regional factions)
- `rules/22-LOCATION-GENERATION.md` (for key locations)

### Example 3: Start a new campaign
**Load:**
- CORE files (rules/01-05)
- `rules/10-SESSION-INITIALIZATION.md` (mode detection)
- `rules/70-CAMPAIGN-FORMAT.md` (format rules)

### Example 5: Run a live session
**Load:**
- CORE files (rules/01-05)
- `rules/52-LIVE-SESSION-MANAGEMENT.md` (live session protocol)
- `rules/50-ENCOUNTER-COMBAT.md` (if combat expected)
- `rules/60-AUDIT-PROTOCOLS.md` (session log auditing)
- `rules/90-TAG-GLOSSARY.md` (tag reference for DM helper tags)
- `rules/91-DM-TIPS-REFERENCE.md` (contextual DM guidance)

### Example 5: Generate treasure hoard or custom magic item
**Load:**
- CORE files (rules/01-05)
- `rules/26-ITEM-GENERATION.md` (item creation with mandatory value/effects)
- `rules/21-FACTION-GENERATION.md` (if item has faction ties)
- `rules/33-REWARD-SYSTEMS.md` (to match item to player desires)
- `rules/33-REWARD-SYSTEMS.md` (player desires)

## Key Features

1. **Four Laws of Interconnection:** Every element must satisfy Causality, Conflict, Secrecy, and Fragility
2. **Plot Web:** Visual summary of connections and tensions between elements
3. **Living Clock:** Factions and NPCs progress independently of player action
4. **Moral Consequence Register:** Tracks harmful actions and their weight
5. **World-Pull:** Ensures world affects players, players affect world
7. **Live Session Facilitation:** Real-time session management with session logs, LLM memory markers, DM helper tags, and combat agency rules
8. **Token Efficiency:** Load only what you need (50-85% token savings)

## Output Requirements

Every generated file must include:
- Table of Contents with anchor links
- Clear section hierarchy
- Cross-references to related files
- DM secrets clearly separated
- Metadata header with world name and date
- Consistent tag system

## Important Notes

- **Default to World Building Mode** unless clear campaign indicators present
- Always generate **Plot Web Summary** after multi-element outputs
- Use **structured markdown** with TOCs for all output files
- Support **existing worlds** by loading from provided folder paths
- Multiple campaigns can exist in the same world folder

## Token Budget Awareness

The full system is ~10,000 tokens. Modular loading reduces this to:
- Micro request (1 NPC): ~2,000 tokens
- Standard request (3-5 elements): ~3,500 tokens
- Full region: ~5,000 tokens

Always prioritize loading only what's needed for the current request.
