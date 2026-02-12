# 🗺️ REGION GENERATION — Layer 1

**[LOAD PRIORITY: ON-DEMAND — Load when generating regions or large-scale geography]**

---

## Layer 1 — The Regions

Regions are the large-scale geographic and cultural containers for campaigns. They establish tone, conflict, and scope. Every region should feel distinct and purposeful.

### Required Components

Each region must include:

- **Name + Aesthetic** — What is this region called and what does it feel like?
- **Primary Conflict** — What tension defines this region?
- **Hidden Truth** — What secret underlies the surface reality?
- **Connection Points** — How does this region link to others?
- **Player Hook** — Why should players care about this region?
- **Scarce Resource** — What does this region lack or contest?
- **Civilization Texture Entry** — Daily life details
- **Linguistic Profile** — How do people speak here?
- **Scale Reference** — Geographic size and travel times
- **Genre Thread Presence** (hybrid genres only) — Which genre threads are active here?

---

## Region Generation Template

```
## [Region Canonical Name]

**Aesthetic:** [What does this region feel/look/sound like?]
Use sensory details and thematic keywords:
- Examples: "windswept moors heavy with fog" / "sun-bleached desert cities of white stone" / "dense industrial sprawl choked with smoke"

**Primary Conflict:** [What tension defines this region right now?]
This should be:
- Observable to players
- Connected to at least one faction
- Actionable (players can engage with it)

Examples:
- "Two merchant guilds war over control of the harbor"
- "Refugees flood the region, straining resources and stirring xenophobia"
- "Ancient ruins awaken, releasing creatures that disrupt settlements"

**Hidden Truth:** [What secret underlies the surface reality?]
Information Tier: [HIDDEN or LOST — never PUBLIC]

Examples:
- "The 'merchant war' is a cover for a supernatural struggle between two archfey"
- "The refugees are fleeing a curse, which they're unknowingly spreading"
- "The ruins were deliberately awakened by a faction seeking ancient weapons"

Tag: `[HIDDEN TRUTH: region X — truth: Y — Information Tier: Z]`

**Connection Points:** [How does this region link to others?]
- **North**: [adjacent region or barrier — travel time]
- **South**: [adjacent region or barrier — travel time]
- **East**: [adjacent region or barrier — travel time]
- **West**: [adjacent region or barrier — travel time]
- **Other**: [planar connections, teleportation circles, sea routes, underground passages]

Tag: `[SPATIAL REF: region X borders region Y to the north — 3 days by horse]`

**Player Hook:** [Why should players care about this region?]
- Connection to PC backstory?
- Resource players need?
- Threat to something players value?
- Opportunity for power, wealth, knowledge, etc.?

Tag: `[PLAY HOOK: region X — draws players via Y]`

**Scarce Resource:** [What does this region lack or contest?]
Examples:
- Water (desert regions)
- Arable land (mountainous regions)
- Political stability (war-torn regions)
- Magic (anti-magic zones)
- Safety (monster-infested regions)
- Knowledge (isolated regions)

This scarcity creates:
- Faction conflict (competing for resource)
- Economic dynamics (trade opportunities)
- Social tension (haves vs have-nots)
- Player opportunity (bring scarce resource, gain leverage)

Tag: `[RESOURCE FAULT: region X lacks Y — creates tension Z]`

**Civilization Texture Entry:**
What does daily life look like here?
- **Common Professions**: [what do most people do for work?]
- **Architecture**: [what are buildings made of? — how do they look?]
- **Food**: [what do people eat here? — local specialties?]
- **Social Customs**: [distinctive traditions, greetings, taboos]
- **Calendar/Festivals**: [when do people celebrate? — why?]

Tag: `[CIVILIZATION TEXTURE: region X — detail: Y]`

See [42-CIVILIZATION-TEXTURE.md](42-CIVILIZATION-TEXTURE.md) for full protocol.

**Linguistic Profile:**
- **Primary Language(s)**: [what languages are spoken here?]
- **Formality Level**: [High / Medium / Low]
- **Distinctive Vocabulary**: [regional terms, slang, idioms]
- **Accent/Dialect Notes**: [pronunciation quirks, grammatical patterns]
- **Code-Switching**: [do people change language/register based on context?]

Tag: `[LINGUISTIC PROFILE: region X — primary language: Y — formality: Z]`

See [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md) for full protocol.

**Scale Reference:**
- **Geographic Size**: [approximate area — compare to real-world if useful]
- **Population**: [approximate number of inhabitants]
- **Travel Times** (internal):
  - [Settlement A] to [Settlement B]: [X days by horse / Y days on foot]
  - [Settlement C] to [Settlement D]: [X days by horse / Y days on foot]
- **Major Settlements**: [list 3-5 key cities, towns, or villages]

Tag: `[SCALE REF: region X — Settlement A to B: 2 days by horse]`

**Genre Thread Presence:** (hybrid genres only)
If running a genre-blended campaign, note which genre threads are active in this region.

Examples:
- High Fantasy + Noir: "This region emphasizes the Noir thread — urban crime, moral ambiguity"
- Gothic Horror + Political Intrigue: "Both threads present — Horror dominates rural areas, Intrigue in the capital"

Tag: `[GENRE THREAD: region X — active thread: Y — status: dominant/balanced/minor]`

See [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) for genre blend maintenance.
```

---

## Region and Faction Integration

Regions should host at least 2 factions with opposing goals. The Primary Conflict often emerges from faction tension.

**Questions to ask**:
- Which factions control resources in this region?
- Which factions contest control?
- Which factions are native vs. foreign?
- Which factions represent the Hidden Truth?

Tag faction presence: `[FACTION PRESENCE: faction X operates in region Y — control level: dominant/contested/covert]`

---

## Region and Location Deployment

Each region should have:
- **Tier 0-1 locations**: 3-5 essential locations (starting city, faction HQs, central landmarks)
- **Tier 2 locations**: 2-3 mid-campaign reveals (hidden bases, restricted areas)
- **Tier 3 locations**: 0-2 late-campaign secrets (ancient ruins, planar gates)

Not all locations need to be generated at region creation — deploy as needed.

---

## Region Progression

Regions are NOT static. They change based on:
- **Faction Clock advancement**: When factions reach Clock Stages, regions reflect changes
- **PC action consequences**: Player choices reshape regions
- **Time passage**: Seasons, disasters, migrations
- **Cross-region ripples**: Events in neighboring regions affect this one

When a region changes significantly:
Tag: `[WORLD STATE UPDATE: region X — previous state: Y — current state: Z — cause: W]`

Examples:
- `[WORLD STATE UPDATE: The Thornlands — previous: contested territory — current: under Syndicate control — cause: Clock Stage 3 success]`
- `[WORLD STATE UPDATE: The Ashmark — previous: habitable farmland — current: smoking wasteland — cause: PC released bound火 demon]`

---

## Scarce Resource as Conflict Engine

The Scarce Resource creates natural faction tension and player opportunity.

**Resource Scarcity Levels**:
- **Abundant**: No conflict; region is self-sufficient
- **Adequate**: Managed carefully; potential for future scarcity
- **Contested**: Multiple factions fight for control; source of Primary Conflict
- **Critical**: Region cannot function without external supply; desperate measures
- **Depleted**: Resource is gone; region faces collapse

Tag: `[RESOURCE FAULT: region X — resource Y — scarcity level: contested]`

**Player Opportunity**:
- Players control resource → leverage over factions
- Players provide resource → gratitude and rewards
- Players destroy resource → faction war escalates
- Players discover hidden resource → shift power dynamics

---

## Multi-Region Campaigns

For campaigns spanning multiple regions:

**Region Contrast**: Each region should feel distinct from others.
- Different aesthetic (desert vs. forest vs. urban)
- Different Primary Conflict (war vs. intrigue vs. survival)
- Different Scarce Resource (water vs. magic vs. safety)
- Different Linguistic Profile (formal vs. colloquial)
- Different Genre Thread emphasis (if hybrid)

**Region Relationships**:
- **Allied**: Trade partners, mutual defense
- **Hostile**: At war or cold war
- **Isolated**: No meaningful contact
- **Dependent**: One region relies on another
- **Colonial**: One region controls another

Tag: `[REGION RELATIONSHIP: region X and Y — type: dependent — X relies on Y for food imports]`

**Travel Between Regions**:
Always specify travel time and method:
- Overland: horse, foot, wagon
- Sea: ship, boat
- Magical: teleportation circles, portals
- Planar: planar gates, divine intervention

Tag: `[SPATIAL REF: region X to Y — 10 days by horse via the King's Road]`

---

## Region and Scale Calibration

**Micro-Scale Regions** (single city or small area):
- Emphasize neighborhoods and districts
- Factions operate at street/local level
- Travel measured in hours or less

**Standard-Scale Regions** (province or territory):
- Emphasize multiple settlements
- Factions operate at local/regional level
- Travel measured in days

**Macro-Scale Regions** (kingdom or continent):
- Emphasize major cities and wilderness areas
- Factions operate at regional/pivotal level
- Travel measured in weeks

---

## Common Region Generation Pitfalls

**Avoid**:
- Regions that are just "generic fantasy land"
- Regions with no internal conflict or faction tension
- Regions that never change regardless of player action
- Regions that all feel the same (no aesthetic/cultural contrast)
- Regions with no scarce resources (eliminates faction conflict drivers)
- Regions with no Hidden Truth (no depth, no mystery)

**Prefer**:
- Regions with distinctive aesthetic and cultural texture
- Regions where faction conflict creates visible tension
- Regions that respond to player actions via World State updates
- Regions with strong aesthetic/cultural contrast from each other
- Regions where resource scarcity drives faction behavior
- Regions where surface reality conceals hidden complexity

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction presence in regions
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Location deployment in regions
- [40-SPATIAL-SYSTEMS.md](40-SPATIAL-SYSTEMS.md) — Spatial reference and travel times
- [42-CIVILIZATION-TEXTURE.md](42-CIVILIZATION-TEXTURE.md) — Daily life details
- [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md) — Regional language profiles
- [71-GENRE-SYSTEMS.md](71-GENRE-SYSTEMS.md) — Genre thread distribution across regions
