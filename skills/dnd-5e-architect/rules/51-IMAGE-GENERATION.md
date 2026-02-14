# 🎨 IMAGE GENERATION PROTOCOLS

**[LOAD PRIORITY: ON-DEMAND — Load only when generating images for worldbuilding elements]**

---

## Purpose

Generate visual representations of NPCs, locations, creatures, and items to enhance worldbuilding immersion.

**When to Generate Images**:
- Major NPCs (recurring characters)
- Key locations (important settings)
- Unique creatures (distinctive monsters)
- Significant items (legendary artifacts)
- Campaign maps and diagrams

**When NOT to Generate**:
- Minor background NPCs
- Generic locations
- Standard monsters from books
- Common items

Tag: `[IMAGE GEN: generate for major NPCs, key locations, unique creatures, significant items]`

---

## Image Generation Format

Use the IMGPROMPT tag to generate images:

### Format

```
[IMGPROMPT: detailed description of visual elements, art style, composition, lighting, mood]
```

**Required Elements**:
- **Subject**: What is being depicted
- **Visual Details**: Appearance, clothing, features
- **Art Style**: Fantasy art, oil painting, digital art, etc.
- **Composition**: Close-up, full body, environment shot
- **Mood/Lighting**: Atmospheric details

**Example**:
```
[IMGPROMPT: A weathered female half-elf ranger in her 40s with silver-streaked dark hair tied back, wearing practical leather armor with forest-green cloak, standing in misty forest clearing at dawn, bow in hand, realistic fantasy art style, atmospheric lighting through trees]
```

Tag: `[IMGPROMPT: subject — visual details — art style — composition — mood]`

---

## NPC Image Prompts

For generating character portraits:

### NPC Portrait Template

```
[IMGPROMPT: [Race] [gender] [age], [distinctive physical features], [clothing/armor description], [pose/expression], [background setting], [art style], [lighting/mood]]
```

**Physical Features to Include**:
- Age (young, middle-aged, elderly)
- Build (slender, muscular, stocky)
- Hair (color, style, length)
- Eyes (color, expression)
- Distinctive marks (scars, tattoos, etc.)
- Facial features (angular, soft, weathered)

**Clothing Details**:
- Type (armor, robes, common clothes)
- Colors and materials
- Condition (pristine, worn, tattered)
- Accessories (jewelry, weapons, tools)

**Examples**:

**Noble NPC**:
```
[IMGPROMPT: Human male in his 50s, distinguished with graying temples and neat beard, wearing elegant burgundy doublet with gold embroidery, fur-trimmed cloak, standing in ornate throne room, confident expression, fantasy portrait art, warm candlelight]
```

**Villain NPC**:
```
[IMGPROMPT: Female tiefling warlock, mid-30s, crimson skin with black horns, piercing yellow eyes, elaborate dark robes with arcane symbols, holding ancient tome, shadowy chamber with floating candles, dark fantasy art style, dramatic rim lighting]
```

**Merchant NPC**:
```
[IMGPROMPT: Stout dwarf male, middle-aged with braided brown beard decorated with coins, wearing practical merchant's vest over sturdy traveling clothes, standing in cluttered shop with goods on shelves, friendly smile, warm fantasy art, cozy interior lighting]
```

Tag: `[NPC IMAGE: character name — portrait with specified features and setting]`

---

## Location Image Prompts

For generating setting visuals:

### Location Image Template

```
[IMGPROMPT: [Location type], [architectural style/natural features], [scale indicators], [atmospheric conditions], [time of day], [key visual elements], [art style], [perspective]]
```

**Elements to Include**:
- Architecture or terrain type
- Size and scale (intimate tavern vs. vast cathedral)
- Building materials (stone, wood, etc.)
- State of repair (pristine, weathered, ruined)
- Population (bustling, empty, abandoned)
- Lighting and weather
- Unique distinguishing features

**Examples**:

**Tavern Interior**:
```
[IMGPROMPT: Cozy medieval tavern interior, low wooden beams, stone fireplace with roaring fire, scattered wooden tables and benches, warm candlelight, patrons in shadows, fantasy tavern art style, intimate perspective from doorway]
```

**Ancient Temple**:
```
[IMGPROMPT: Massive stone temple interior, towering columns carved with ancient runes, shafts of dusty sunlight through high windows, cracked marble floors, enormous statue at far end, fantasy architecture art, dramatic perspective looking up]
```

**Wilderness Location**:
```
[IMGPROMPT: Misty forest clearing with ancient standing stones arranged in circle, moss-covered and carved with faded symbols, surrounded by towering old-growth trees, early morning fog, fantasy landscape art, wide atmospheric shot]
```

**Urban Scene**:
```
[IMGPROMPT: Bustling medieval market square, colorful merchant stalls with awnings, crowds of people, half-timbered buildings surrounding plaza, fountain at center, midday sun, fantasy city art style, bird's eye perspective]
```

Tag: `[LOCATION IMAGE: location name — setting with specified atmosphere and features]`

---

## Creature Image Prompts

For generating monster/creature visuals:

### Creature Image Template

```
[IMGPROMPT: [Creature type], [size], [distinctive features], [pose/action], [environment], [threat level indicators], [art style], [perspective]]
```

**Elements to Include**:
- Base creature type
- Size (tiny to gargantuan)
- Unique features (mutations, magical effects)
- Pose (threatening, wounded, idle)
- Environmental context
- Combat-ready or neutral

**Examples**:

**Standard Monster**:
```
[IMGPROMPT: Large corrupted wolf with matted black fur, glowing red eyes, exposed fangs, unnatural proportions, crouched in aggressive stance, dark forest background, fog swirling around paws, dark fantasy creature art, low angle shot]
```

**Unique Boss Creature**:
```
[IMGPROMPT: Colossal skeletal dragon wreathed in green ghostfire, tattered wings, eye sockets glowing with necromantic energy, perched atop ruined castle tower, stormy night sky with lightning, epic fantasy art style, dramatic upward angle]
```

**Friendly Creature**:
```
[IMGPROMPT: Small fey dragon, iridescent butterfly wings, playful expression, perched on flowering branch, enchanted forest glade with sparkles of magic in air, whimsical fantasy art style, close-up perspective]
```

Tag: `[CREATURE IMAGE: creature name — appearance with threat level and setting]`

---

## Item Image Prompts

For generating artifact/item visuals:

### Item Image Template

```
[IMGPROMPT: [Item type], [materials], [decorative elements], [magical effects], [scale reference], [background], [art style], [lighting]]
```

**Elements to Include**:
- Item type and shape
- Materials (metals, gems, wood, etc.)
- Craftsmanship quality
- Magical effects or glowing elements
- Age and condition
- Cultural design influences

**Examples**:

**Magic Weapon**:
```
[IMGPROMPT: Longsword with ornate crossguard shaped like dragon wings, blade etched with glowing blue runes, pommel set with sapphire, displayed on dark velvet background, fantasy weapon art, dramatic spotlight]
```

**Artifact**:
```
[IMGPROMPT: Ancient crown made of silver and black metal, set with star-like diamonds, arcane symbols carved along band, faint ghostly aura, resting on stone pedestal in misty chamber, legendary artifact art style, mystical lighting]
```

**Common Item with Significance**:
```
[IMGPROMPT: Worn leather journal with brass clasp, pages yellowed with age, mysterious symbols on cover, sitting on wooden desk with scattered quills and ink, warm candlelight, realistic fantasy still life art]
```

Tag: `[ITEM IMAGE: item name — design with materials and magical properties]`

---

## Map Generation Prompts

For generating visual maps:

### Map Template

```
[IMGPROMPT: [Map type], [art style], [scale], [key locations labeled], [terrain features], [borders], [legend elements], [artistic embellishments]]
```

**Map Types**:
- Region map (large scale)
- City map (medium scale)
- Building floor plan (small scale)
- Battle map (tactical grid)
- World map (continental scale)

**Examples**:

**Regional Map**:
```
[IMGPROMPT: Fantasy region map showing forested mountains to north, coastal city to south, river running through center, roads connecting towns, hand-drawn cartography style, aged parchment texture, compass rose, decorative border, labeled locations]
```

**City Map**:
```
[IMGPROMPT: Medieval city map with districts marked by different colors, walls and gates, landmarks labeled, harbor district on waterfront, castle in center, parchment-style fantasy cartography, birds-eye view, scale indicator]
```

**Dungeon Map**:
```
[IMGPROMPT: Underground dungeon map, stone corridors and chambers, grid overlay for tactical use, room numbers, trap and secret door symbols, black and white sketch style, 20 rooms spread across two levels, stairs connecting]
```

Tag: `[MAP IMAGE: map type covering specified area with key features]`

---

## Art Style Guidelines

Different styles for different elements:

### Recommended Styles

**Character Portraits**:
- "realistic fantasy portrait art"
- "digital fantasy character art"
- "oil painting character portrait"

**Locations**:
- "fantasy landscape art"
- "concept art environment"
- "matte painting style"

**Creatures**:
- "dark fantasy creature design"
- "monster concept art"
- "digital creature illustration"

**Items**:
- "fantasy weapon concept art"
- "artifact illustration"
- "still life fantasy art"

**Maps**:
- "hand-drawn fantasy cartography"
- "aged parchment map style"
- "artistic world map"

Tag: `[ART STYLE: realistic fantasy portrait art for NPCs, concept art for locations]`

---

## Mood and Lighting

Set emotional tone through lighting:

**Light/Hopeful**:
- "warm sunlight"
- "golden hour lighting"
- "bright and airy"

**Dark/Ominous**:
- "shadowy with rim lighting"
- "dark atmosphere"
- "sinister lighting"

**Mysterious**:
- "misty and atmospheric"
- "fog-shrouded"
- "ethereal lighting"

**Dramatic**:
- "dramatic spotlight"
- "chiaroscuro lighting"
- "high contrast"

**Cozy/Safe**:
- "warm candlelight"
- "firelight glow"
- "soft interior lighting"

Tag: `[MOOD: dramatic spotlight for villain, warm candlelight for friendly tavern]`

---

## Perspective and Composition

Frame the image effectively:

**Portrait**:
- "close-up face shot"
- "head and shoulders portrait"
- "full body portrait"

**Location**:
- "wide establishing shot"
- "interior perspective"
- "bird's eye view"

**Creature**:
- "low angle looking up (threatening)"
- "eye level confrontation"
- "full body creature shot"

**Action**:
- "dynamic action pose"
- "mid-combat shot"
- "dramatic moment"

Tag: `[COMPOSITION: low angle for threatening boss, eye level for NPC portraits]`

---

## Cultural and Aesthetic Details

Make visuals culturally distinctive:

**Architecture**:
- "Gothic spires and arches"
- "Eastern-inspired pagoda design"
- "Nomadic tent structures"
- "Dwarven stone architecture"

**Clothing**:
- "Renaissance-era fashion"
- "Tribal war paint and furs"
- "Oriental silk robes"
- "Nordic fur-trimmed armor"

**Weapons/Items**:
- "Celtic knotwork designs"
- "Japanese-inspired blade"
- "Tribal bone decorations"
- "Baroque ornate detailing"

Tag: `[CULTURAL AESTHETIC: Gothic architecture for vampire castle, Celtic knotwork for druid items]`

---

## Avoiding Generic Images

Make images distinctive:

**Add Specific Details**:
❌ "A wizard"
✅ "An elderly wizard with star-patterned blue robes and owl familiar perched on staff"

**Include Story Elements**:
❌ "A sword"
✅ "A chipped sword with blood-red gems in crossguard, blade covered in old battle scars"

**Set Mood**:
❌ "A forest"
✅ "A mist-shrouded ancient forest with bioluminescent mushrooms and twisted trees"

**Cultural Context**:
❌ "A city"
✅ "A desert city with white sandstone buildings, blue-tiled domes, and market awnings in ochre and turquoise"

Tag: `[DISTINCTIVE DETAILS: include specific features, story elements, mood, cultural context]`

---

## Image Consistency

Maintain visual consistency across campaign:

**Style Consistency**:
- Use same art style for all portraits
- Same map style for all maps
- Consistent color palette

**Character Consistency**:
- If generate NPC image, reference it in future descriptions
- Keep visual details consistent
- Update image if character changes significantly

**World Consistency**:
- Architecture style consistent within culture
- Technology level consistent
- Color schemes for factions consistent

Tag: `[IMAGE CONSISTENCY: maintain same art style, color palettes, design language across all generated images]`

---

## When Not to Generate Images

Some things better left to imagination:

**Skip Images For**:
- Ultra-gory violence
- Intimate adult content
- Generic background NPCs (merchants, guards)
- Standard D&D monsters (use book art)
- Every single room in dungeon

**Prioritize Images For**:
- Major campaign NPCs (party sees regularly)
- Unique locations (campaign-central places)
- Original monsters (homebrewed creatures)
- Important artifacts (plot-significant items)
- Regional maps (orientation and reference)

Tag: `[IMAGE PRIORITY: focus on major NPCs, key locations, unique creatures, significant items]`

---

## Image Integration with Generation

When to include image prompts in generation:

**Include IMGPROMPT When**:
- Generating major NPC (include at end of generation)
- Generating key location (include in Location Register)
- Generating unique creature (include with stat block)
- Generating significant item (include with item description)

**Format in Generation**:
```
[NPC Name, Layer 3]
[Full generation content...]

**Visual Reference:**
[IMGPROMPT: detailed image description based on generated details]
```

Tag: `[IMAGE INTEGRATION: include IMGPROMPT at end of major generations]`

---

## Revising Image Prompts

If first generation isn't right, revise prompt:

**Common Issues**:
- Too generic → Add more specific details
- Wrong mood → Adjust lighting and atmosphere words
- Wrong composition → Specify perspective/framing
- Missing key detail → Add explicit mention

**Revision Example**:
```
First attempt:
[IMGPROMPT: A wizard in a tower]

Revised:
[IMGPROMPT: Elderly male human wizard with long white beard and star-patterned midnight blue robes, reading ancient tome at desk in circular stone tower room, owl familiar perched on shoulder, walls lined with bookshelves, warm candlelight, atmospheric fantasy art, intimate perspective]
```

Tag: `[IMAGE REVISION: add specificity, mood, perspective if initial prompt too vague]`

---

## Common Image Generation Mistakes

❌ **Too vague** — "A knight" (hundreds of variations)
✅ **Specific** — "Female half-orc knight in battle-worn plate armor with clan symbols"

❌ **Too complex** — Trying to fit entire scene with 10 characters
✅ **Focused** — One or two characters, clear subject

❌ **Missing mood** — No lighting or atmosphere description
✅ **Atmospheric** — Specify lighting, weather, time of day

❌ **Inconsistent style** — Different art styles across campaign
✅ **Consistent** — Same style descriptor for all images

❌ **Generic fantasy** — Could be from any setting
✅ **Setting-specific** — Include distinctive cultural/world details

---

**See also:**
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — NPC details for portrait generation
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Location sensory details for scene generation
- [23-CREATURE-GENERATION.md](23-CREATURE-GENERATION.md) — Creature descriptions for monster art
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — Tag library including IMGPROMPT
