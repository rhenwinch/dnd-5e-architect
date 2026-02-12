# 🧭 SESSION INITIALIZATION

**[LOAD PRIORITY: STARTUP — Required for new campaigns and worlds]**

---

## Mode Detection

**FIRST STEP:** Determine if this is World Building or Campaign Mode.

### Detection Logic

**Indicators of CAMPAIGN MODE:**
- User mentions: "my players", "our session", "PC named X did Y", "last session"
- Active session context ("we're playing tonight")
- Player character names with actions
- References to ongoing campaign state

**Indicators of WORLD BUILDING MODE:**
- "Create a world", "build a setting", "I need a region"
- No mention of active players or sessions
- Requests for reusable content
- "For future campaigns" or "standalone world"

**If Uncertain:**
Ask directly: *"Are you building a world (for potential future campaigns) or running an active campaign with players?"*

**Default:** If no clear indicators, assume **WORLD BUILDING MODE**.

---

## World Building Mode Initialization

**When activated:** Creating standalone world content for potential future use.

**Check for Existing World:**
- Ask: *"Are you creating a new world or adding to an existing one?"*
- If existing: *"What's the world name/folder?"*
- Load existing world files from `worlds/[world-name]/` if present

**Gather World Parameters:**

1. **World Name**
   - lowercase-with-hyphens format
   - This becomes the folder name

2. **Genre / Tone**
   - Fantasy subgenre or tone
   - Default: Classic D&D 5e High Fantasy if not specified

3. **Geographic Scope**
   - Single city, region, continent, world, multiverse?

4. **Initial Context** (Optional)
   - Past history, major events, or established world facts
   - Provides foundation without constraining future campaigns
   - Examples: "Ancient empire fell 500 years ago", "Magic recently returned", "Three moons orbit this world"

5. **Established Facts** (if adding to existing world)
   - Load existing world files
   - Review canon from readme and timeline

**Output Structure:**
- Save to `worlds/[world-name]/[world-name]-[type].md`
- Create readme.md with world overview
- Tag as `[MODE: World Building]`

---

## Campaign Mode Initialization

**When activated:** Running active campaign with players.

**Check for Existing World:**
- Ask: *"Are you using an existing world or creating a new one?"*
- If existing world folder provided:
  - Load world files from `worlds/[world-name]/`
  - Create campaign subfolder: `worlds/[world-name]/campaigns/[campaign-name]/`
- If new world needed:
  - Run World Building Mode initialization first
  - Then proceed with campaign setup

**Gather Campaign Parameters:**

1. **Campaign Name**
   - lowercase-with-hyphens format
   - Becomes subfolder under world

2. **World Context**
   - Which world folder to use
   - Load existing world canon

3. **Campaign Premise**
   - Use Layer 0 format: *"[Powerful force] threatens [something valued], because [hidden reason], unless [player-shaped outcome]."*
   - This defines the SPECIFIC story for this campaign
   - Different campaigns in same world can have different premises

4. **Player Characters**
   - Names, races, classes, visible backgrounds
   - Do NOT request full backstories (Backstory Embargo)

5. **Player Count & Experience**

6. **Campaign Format** — One-Shot / Short Arc / Full Campaign

7. **Player Desire Profile**

**Output Structure:**
- World elements → `worlds/[world-name]/[world-name]-[type].md`
- Campaign elements → `worlds/[world-name]/campaigns/[campaign-name]/[campaign-name]-[type].md`
- Tag as `[MODE: Campaign — World: world-name]`

---

## Additional Parameters (Both Modes)

Regardless of mode, gather these when relevant:

1. **Genre Blend Declaration** (if hybrid)
   - If mixing genres, declare all active threads
   - Example: "High Fantasy + Noir" or "Gothic Horror + Political Intrigue"
   - See [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) for blend maintenance

2. **Default Request Scope**
   - Micro (single element), Standard (3-5 elements), or Full (complete region)?
   - Can be adjusted per request
   - See Request Scope Calibration in [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md)

3. **Table Use Mode**
   - Live session, prep between sessions, or solo worldbuilding?
   - Determines pacing and detail level

4. **Image Style Preference** (if using visual generation)
   - Art style: Realistic, painterly, sketch, comic, etc.
   - Color palette preferences
   - See [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md)

10. **Image Style Preference** (if using visual generation)
    - Art style: Realistic, painterly, sketch, comic, etc.
    - Color palette preferences
    - See [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md)

11. **Table Use Mode**
    - Live session, prep between sessions, or solo worldbuilding?
    - Determines pacing and detail level

12. **Default Request Scope**
    - Micro (single NPC/location), Standard (3-5 elements), or Full (complete region)?
    - Can be adjusted per request
    - See Request Scope Calibration in [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md)

13. **Genre Blend Declaration** (if hybrid)
    - If mixing genres, declare all active threads
    - Example: "High Fantasy + Noir" or "Gothic Horror + Political Intrigue"
    - See [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) for blend maintenance

---

## Layer 0 — The Premise

Every world begins with a premise. Format:

> *"[Powerful force] threatens [something valued], because [hidden reason], unless [player-shaped outcome]."*

**Examples:**
- *"A lich-king's curse threatens the kingdom's harvest, because he seeks to starve the living into undeath, unless heroes break the phylactery hidden in Death's Garden."*
- *"Corporate mages threaten the city's water supply, because they profit from bottling potable water, unless citizens expose the contamination conspiracy."*
- *"A forgotten god threatens reality's coherence, because it was erased from all memory and seeks existence, unless mortals remember its true name."*

The premise is:
- **Speculative until confirmed** — tag as `[SPECULATIVE]` if not agreed upon
- **Player-shapeable** — the "unless" clause is never predetermined
- **Hidden-truth-aware** — the "because" reveals something not immediately obvious

---

## After Initialization

Once parameters are gathered:
1. Generate Layer 1 (Regions) if world-scale
2. Generate Layer 2 (Factions) — minimum 2, recommended 3-4
3. Generate Layer 3 (NPCs) — populate faction faces and key contacts
4. Generate Layer 4 (Locations) — initial deployment tier locations
5. Establish Living Clock entries for major factions
6. Create initial Plot Web showing faction tensions

Tag the initialized state:
`[WORLD STATE: Initialized — Format: X — Genre: Y — Premise: Z]`

---

**See also:**
- [02-CORE-WORLDBUILDING-PHILOSOPHY.md](02-CORE-WORLDBUILDING-PHILOSOPHY.md) — Operational modes explained
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — File organization structure
- [25-REGION-GENERATION.md](25-REGION-GENERATION.md) — Layer 1 generation
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Layer 2 generation
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — Layer 3 generation
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Layer 4 generation
- [70-CAMPAIGN-FORMAT.md](70-CAMPAIGN-FORMAT.md) — Format-specific rules
