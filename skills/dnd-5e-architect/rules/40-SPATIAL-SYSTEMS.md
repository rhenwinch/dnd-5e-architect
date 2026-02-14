# 🗺️ SPATIAL SYSTEMS

**[LOAD PRIORITY: ENHANCEMENT — Load when working with detailed geography, positioning, or travel]**

---

## Spatial Anchor Rule

Every location must have a **spatial reference** — position relative to other locations with travel time.

This creates navigable space and helps players form mental maps.

### Format

`[SPATIAL REF: location X — direction from Y — travel time by Z method]`

### Examples

- `[SPATIAL REF: The Archive — 3 blocks east of Market Square — 10 minutes on foot]`
- `[SPATIAL REF: Death's Garden — 5 days north of the Capital by horse — through Thornwood Forest]`
- `[SPATIAL REF: The Undercroft — 200 feet below the Guild Hall — 1 hour descent via stairs]`

---

## Scale Reference System

Regions need internal scale references to establish geographic scope and travel times.

### Format

```
**Scale Reference:**
- **Geographic Size**: [approximate area — compare to real-world if useful]
- **Population**: [approximate number of inhabitants]
- **Travel Times** (internal):
  - [Settlement A] to [Settlement B]: [X days by horse / Y days on foot]
  - [Settlement C] to [Settlement D]: [X days by horse / Y days on foot]
- **Major Settlements**: [list 3-5 key cities, towns, or villages]

Tag: [SCALE REF: region X — Settlement A to B: 2 days by horse]
```

---

## Travel Time Standards

Establish consistent travel speeds for different methods:

| Method | Speed | Terrain Notes |
|---|---|---|
| **On foot** | ~20 miles/day | Paved roads, good weather |
| **On foot (difficult)** | ~10 miles/day | Wilderness, mountains, poor weather |
| **Horse** | ~30-40 miles/day | Paved roads, good weather |
| **Horse (difficult)** | ~15-20 miles/day | Wilderness, mountains |
| **Wagon** | ~15-20 miles/day | Roads only, slower than horse |
| **Ship (river)** | ~30-50 miles/day | Downstream faster, upstream slower |
| **Ship (sea)** | ~50-100 miles/day | Wind-dependent, weather-dependent |

**Use these as baselines**, then adjust for world-specific factors.

---

## Directional References

Always specify direction when positioning locations relative to each other:

**Cardinal Directions**: N, S, E, W, NE, NW, SE, SW

**Examples**:
- "The Archive is 3 blocks **east** of Market Square"
- "Death's Garden lies **5 days north** of the Capital"
- "The mountains are **to the west**, the sea **to the east**"

Avoid vague references like "near" or "close to" — always give distance and direction.

---

## Landmarks and Wayfinding

Locations should reference **visible landmarks** that help with navigation:

**Examples**:
- "The tavern is beneath the clock tower — you can see the tower from anywhere in the district"
- "Look for the red bridge; the blacksmith is on the north side"
- "The ruins are visible from the road — three ancient spires rising above the trees"

Tag: `[LANDMARK: location X — visible feature: Y — visible from: Z]`

---

## Vertical Positioning

Don't forget the Z-axis! Some locations are above or below others:

**Above Ground**:
- "The mage's tower is 200 feet tall — 10 floors"
- "The skybridge connects the two buildings at the fourth floor"

**Below Ground**:
- "The catacombs extend 100 feet below street level"
- "The vault is three levels down, behind the sealed door"

Tag: `[SPATIAL REF: location X — 100 feet below location Y]`

---

## Region Borders and Boundaries

When defining regions, specify what lies between them:

**Natural Boundaries**:
- Rivers, mountains, forests, deserts, seas
- "The Thornwood River marks the eastern border"

**Political Boundaries**:
- Treaties, walls, checkpoints
- "The treaty line follows the old stone markers"

**Transition Zones**:
- Borderlands that belong to neither region clearly
- "The Contested Moors — claimed by both kingdoms, controlled by neither"

Tag: `[SPATIAL REF: region X borders region Y — boundary: Thornwood River]`

---

## Map Consistency

If you're generating a physical map or mental map:

1. **Fix cardinal directions** — north is always north
2. **Maintain scale** — distances should be internally consistent
3. **Respect geography** — rivers flow downhill, mountains create barriers
4. **Track travel routes** — roads, rivers, paths should connect logically

---

## Connection Points

Regions connect through:

**Overland Routes**:
- Roads (fastest, safest, trafficked)
- Wilderness paths (slower, dangerous, hidden)
- Mountain passes (seasonal, difficult)

**Water Routes**:
- Rivers (one-way often, bridges are chokepoints)
- Sea lanes (weather-dependent, requires ships)
- Canals (controlled, may require tolls)

**Special Routes**:
- Teleportation circles (expensive, limited locations)
- Planar gates (dangerous, unstable)
- Underground passages (secret, often monster-infested)

Tag: `[CONNECTION POINT: region X to Y — route: King's Road — travel time: 3 days by horse]`

---

## Deployment and Discovery

Not all locations should be revealed immediately. Use **Deployment Tiers**:

**Tier 0**: Already established (players know it exists and how to get there)
**Tier 1**: Early reveal (shown on maps, NPCs mention it)
**Tier 2**: Mid reveal (discovered through investigation or exploration)
**Tier 3**: Late reveal (secret locations requiring keys, knowledge, or relationships)

Tag: `[DEPLOY TIER: 0/1/2/3]`

When promoting a location to earlier tier:
Tag: `[DEPLOY PROMOTION: location X — from Tier 3 to Tier 1 — reason: player action Y]`

---

## Dynamic Geography

Locations can change position or accessibility:

**Seasonal Changes**:
- Mountain passes close in winter
- Rivers flood in spring
- Desert routes only safe at night

**Event-Driven Changes**:
- Bridges destroyed in war
- New roads built by factions
- Magical barriers raised or lowered

When geography changes:
Tag: `[SPATIAL UPDATE: route X — was: passable — now: blocked — reason: bridge destroyed]`

---

## Common Spatial Mistakes to Avoid

❌ **"Near" without specifics** — "The tavern is near the market" (How near?)
✅ **Specific** — "The tavern is 2 blocks north of the market, 5-minute walk"

❌ **Impossible distances** — "The journey is 1 day, no wait, it's 3 days"
✅ **Consistent** — Use travel speed standards, stick to them

❌ **Directions that don't add up** — "Go north to A, then north to B, then north back to A"
✅ **Logical** — If you go north, you must go south to return

❌ **No reference points** — "The ruins are somewhere in the forest"
✅ **Referenced** — "The ruins are 2 days northeast of the village, past the old oak tree"

---

**See also:**
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Spatial Reference in location generation
- [25-REGION-GENERATION.md](25-REGION-GENERATION.md) — Scale Reference and region borders
- [42-CIVILIZATION-TEXTURE.md](42-CIVILIZATION-TEXTURE.md) — How travel affects daily life
