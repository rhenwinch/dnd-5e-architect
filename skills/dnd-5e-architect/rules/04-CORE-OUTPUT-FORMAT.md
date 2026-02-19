# 📤 CORE OUTPUT FORMAT

**[LOAD PRIORITY: CORE — Always Required]**

---

## File Organization Structure

### Directory Structure

All generated content MUST follow this file organization:

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
    └── campaigns/
        └── [campaign-name]/
            ├── [campaign-name]-readme.md
            ├── [campaign-name]-pcs.md
            ├── [campaign-name]-session-log.md
            ├── [campaign-name]-plot-web.md
            └── [campaign-name]-canon.md
```

### File Organization Rules

1. **World Name Format:** lowercase-with-hyphens (e.g., `shadow-crown-empire`)
2. **File Name Format:** `[world-name]-[type].md` (all lowercase)
3. **Campaign Subfolder:** All campaigns exist under `worlds/[world-name]/campaigns/`
4. **Existing World Support:** If user provides existing world folder, use that structure and add campaign subfolder
5. **Cross-References:** Use relative paths between files (e.g., `see [NPCs](world-name-npcs.md)`)

### World Building Mode Output
- Save to `worlds/[world-name]/[world-name]-[type].md`
- Create only the files needed for generated content
- Do NOT create campaign-specific files

### Campaign Mode Output
- Save world elements to `worlds/[world-name]/[world-name]-[type].md`
- Save campaign-specific elements to `worlds/[world-name]/campaigns/[campaign-name]/[campaign-name]-[type].md`
- Campaign files reference world files but do NOT duplicate world content

---

## Structured Output Requirements

Every generated .md file MUST include:

### 1. Table of Contents
```markdown
## Table of Contents
- [Section 1](#section-1)
- [Section 2](#section-2)
  - [Subsection 2.1](#subsection-21)
```

### 2. Clear Section Hierarchy
- Use `##` for major sections
- Use `###` for subsections
- Use `####` for detailed breakdowns
- Maintain consistent heading structure

### 3. Cross-References
- Link to related files: `[Faction Name](WORLD-NAME-FACTIONS.md#faction-name)`
- Link to related sections within same file: `[NPC Name](#npc-name)`
- Use descriptive link text, not bare URLs

### 4. DM Secrets Separation
- Public information in main sections
- Hidden truths in clearly marked subsections:
  ```markdown
  ### Hidden Truth
  > `[HIDDEN]` The actual secret information here...
  ```

### 5. Metadata Headers
Each file should start with:
```markdown
# [World Name] — [Type]
**World:** [world-name] | **Updated:** [date] | **Format:** [campaign format]
```

---

## Header Structure

Use proper Markdown formatting:
- `##` headers for major elements
- `>` blockquotes for hidden truths and speculative content

---

## Tag Library

Full tag library for consistent worldbuilding documentation:

`[SPECULATIVE]`, `[PLAYER-DEFINED]`, `[FLEXIBLE]`, `[INTENTIONAL TROPE]`, `[TONAL OUTLIER]`,
`[PLAY HOOK]`, `[PUBLIC]`, `[RUMORED]`, `[RESTRICTED]`, `[HIDDEN]`, `[LOST]`, `[CONFIRMED CANON]`,
`[DESIRE ANCHOR: X]`, `[CLOCK EVENT: Stage X of Y]`, `[MAGIC: X]`,
`[THREAT TIER: X]`, `[PC ACTION — X]`, `[FAULT LINE: X]`, `[REWARD SOURCE: X]`,
`[CONSEQUENCE OF PC ACTION — X]`, `[RESOURCE SHIFT: X]`, `[TIER ESCALATION: X]`,
`[TIER SIGNAL: X]`, `[RESOURCE FAULT: X]`, `[NPC TRAJECTORY EVENT: X]`,
`[LOCATION CONSEQUENCE: X]`, `[PROPHECY LAYER: X]`, `[REVELATION STAGE: X]`,
`[WORLD STATE UPDATE: X]`, `[ACTIVE THREAD: X]`, `[THREAD RESOLVED: X]`,
`[DM TIP: X]`, `[RP NOTE: X]`, `[SENSORY SIGNATURE: X]`,
`[ALIGNMENT NOTE: X]`, `[INTENTIONAL TONAL CONTRAST]`, `[LEGACY ECHO: X]`,
`[VOICE REGISTER: X]`, `[VOICE REGISTER COLLISION: X]`, `[SCENE REGISTER: X]`,
`[SPEECH REGISTER: X]`, `[LINGUISTIC PROFILE: X]`, `[DIALECT: X]`,
`[OBJECT OWNER: X]`, `[DESIRE RESOLUTION: X]`, `[DESIRE GAP: X]`, `[DESIRE CONFLICT: X]`,
`[DEPTH FLAG: X]`, `[AGENT: X]`, `[WORLD-PULL: X]`,
`[STAKES: Pivotal/Significant/Local/Street]`,
`[POWER ASYMMETRY: X]`, `[MORAL ASYMMETRY: X]`, `[SYMMETRIC CONFLICT: X]`,
`[MORAL CONSEQUENCE: action X — harm to Y — known by Z — weight: W]`,
`[KNOWLEDGE PATH: Primary/Secondary]`, `[CONTESTED KNOWLEDGE]`,
`[ROLEPLAY ACCESS: X — no dice required]`,
`[CANONICAL NAME: X — alias: Y]`, `[NAME LOCK VIOLATION: X → Y]`,
`[WORLD-PULL DEFICIT: X]`, `[KNOWLEDGE BOTTLENECK: X]`, `[CONFLICT STAKES: X]`,
`[FACTION TYPE: Formal/Informal/Emergent]`, `[FACTION EVOLUTION: X → Y]`,
`[FACTION RELATIONSHIP: A ↔ B — history: Z]`, `[FACTION RELATIONSHIP SHIFT: X]`,
`[FACTION RELATIONSHIP RIPPLE: X]`,
`[FACTION GOAL: Pursuing/Consolidating/Defending/Transforming]`,
`[FACTION GOAL SHIFT: X]`,
`[NPC DEPTH: Full/Sketch/Background]`, `[SYMPATHY SIGNAL: X]`,
`[NPC CONSOLIDATED: A + B → C]`, `[NPC RETIRED: X]`,
`[TEMPORAL: X]`, `[CALENDAR REF: X]`,
`[DEPLOY TIER: 0/1/2/3]`, `[DEPLOY PROMOTION: X]`,
`[CONSEQUENCE: PENDING/ACTIVE/RELEASED]`,
`[INACTION CONSEQUENCE: element X — sessions unengaged: Y — micro-advance: Z]`,
`[PC IDENTITY: X]`, `[WORLD OPINION: X]`,
`[PC BACKSTORY HOOK: X]`, `[BACKSTORY ECHO: X]`, `[BACKSTORY ECHO ENCOUNTERED: X]`,
`[RULE CONFLICT RESOLVED: X]`,
`[HOOK TYPE: X]`, `[HOOK INDEPENDENT]`, `[HOOK PREREQ: X — bypass: Y]`,
`[HOOK CHAIN DEPTH: X]`, `[HOOK TYPE GAP: X]`,
`[WORLD TICK: X]`,
`[CANON ARCHAEOLOGY: activating/paying off/retiring X]`,
`[IMGPROMPT: TYPE — prompt text]`,
`[SCENE CARD: X]`, `[SCENE CARD OUTDATED: X]`,
`[CIVILIZATION TEXTURE: X]`, `[CIVILIZATION TEXTURE ACTIVATED: X]`,
`[SCOPE: Micro/Standard/Full]`,
`[BACKSTORY: EMBARGOED — DM only]`,
`[RESOLUTION PATH: Combat — X]`, `[RESOLUTION PATH: Non-Combat — X]`,
`[RESOLUTION PATH: Unexpected — X]`,
`[REWARD ECHO: X]`, `[REWARD TYPE: X — serves desire: Y]`,
`[VILLAIN SUCCESS FOOTPRINT: Clock Stage X — change: Y]`,
`[VISIT REGISTER: location X — visit Y — familiarity: Z]`,
`[EMOTIONAL BEAT: Rising/Peak/Recovery]`,
`[EMOTIONAL ARC: session X — Rising/Peak/Recovery]`,
`[SPATIAL REF: location X — N/S/E/W of Y: travel time Z]`,
`[SCALE REF: region X — Settlement A to B: travel time Y]`,
`[CAMPAIGN FORMAT: One-Shot/Short-Arc/Full-Campaign]`,
`[FORMAT RULE INACTIVE: X]`,
`[GENRE THREAD: X — last appeared: Y — status: Z]`, `[GENRE THREAD FADE: X]`,
`[COSMIC ELEMENT: X — type: Y]`,
`[COSMIC RESOURCE: X]`, `[COSMIC INSTRUMENT: X]`, `[COSMIC CLOCK: age-scale]`,
`[BATTLEFIELD ACTION: Tell — X]`, `[BATTLEFIELD ACTION: Resolution — Y]`,
`[BA NEUTRALIZE: condition X]`, `[BA MITIGATE: condition Y — reduced effect: Z]`,
`[MODE: World Building]`, `[MODE: Campaign — World: world-name]`,
`[OUTPUT PATH: worlds/world-name/FILE.md]`, `[OUTPUT PATH: worlds/world-name/campaigns/campaign-name/FILE.md]`,
`[SANDBOX: open-world design — situations prepped, not stories]`,
`[SANDBOX TYPE: Linear/Non-Linear]`,
`[SETTING SCOPE: Multiple Regions/Single Region — region(s): X]`,
`[LAZY DM PREP: steps completed — session X]`,
`[PREP DEPTH: Layer 1/2/3/4 — session range]`,
`[SANDBOX AUDIT: world/module — pass/fail — missing elements]`,
`[SANDBOX FORMAT: One-Shot/Short-Arc/Full-Campaign — active situations: X]`

---

## Response Endings

- Always end multi-element outputs with **Plot Web Summary**
- Always end session responses with:
  > *"🧩 World Canon Updated. What would you like to expand next?"*

---

**See also:**
- [90-TAG-GLOSSARY.md](90-TAG-GLOSSARY.md) — Complete tag definitions and usage examples
- [72-SANDBOX-PREP.md](72-SANDBOX-PREP.md) — Sandbox prep tags and layered depth model
