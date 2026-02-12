# 🏛️ CIVILIZATION TEXTURE

**[LOAD PRIORITY: ENHANCEMENT — Load when adding daily life detail, customs, festivals, cultural depth]**

---

## Why Texture Matters

Texture is the **daily life details** that make a world feel lived-in:
- What people eat, wear, celebrate
- How they greet each other, resolve disputes, mark time
- Small customs that signal "this is a real place"

Without texture, locations feel like stage sets.
With texture, locations feel like home.

---

## Civilization Texture Entry (for Regions)

Every region should include a **Civilization Texture Entry** — snapshot of daily life.

### Format

```
**Civilization Texture:**
- **Daily Life**: [typical day for common person]
- **Food/Drink**: [local cuisine, staple foods, special dishes]
- **Clothing**: [typical garments, status markers, seasonal changes]
- **Greetings**: [how people say hello, part, show respect]
- **Timekeeping**: [how people mark hours, days, seasons]
- **Currency**: [what's used for trade beyond gold]
- **Festivals**: [major celebrations, holy days, seasonal events]
- **Taboos**: [what's forbidden, offensive, or unlucky]

Tag: [CIVILIZATION TEXTURE: region X — food: Y, greetings: Z, taboo: A]
```

---

## Daily Life

What does a normal day look like for an average person?

**Structure a day**:
- **Dawn**: Day begins when? What's first activity?
- **Morning**: Work, trade, chores?
- **Midday**: Meal? Rest? Community gathering?
- **Afternoon**: More work? Social time?
- **Evening**: When does work end? Dinner? Entertainment?
- **Night**: When do people sleep? Night activities?

**Example (Farming Village)**:
- Dawn: Wake with rooster crow, tend livestock
- Morning: Field work, planting or harvesting
- Midday: Communal meal at village center
- Afternoon: Crafts, repairs, more field work
- Evening: Family dinner, storytelling by fire
- Night: Early to bed, except festival nights

**Example (Urban Merchant District)**:
- Dawn: Shops open at sunrise bell
- Morning: Market rush, busy trading
- Midday: Lunch at stalls, guild meetings
- Afternoon: Quieter sales, accounting
- Evening: Taverns fill, deal-making
- Night: Watch patrols, late-night taverns stay open

Tag: `[DAILY RHYTHM: location X — day begins at dawn bell, market rush midday, taverns fill at dusk]`

---

## Food and Drink

What people eat defines culture:

**Staple Foods**:
- What's the base? (Bread, rice, potatoes, fish?)
- How is it prepared? (Baked, boiled, fried?)
- Eaten when? (Every meal, special occasions?)

**Local Cuisine**:
- Distinctive dishes that signal region
- Ingredients unique to the area
- Preparation methods passed down generations

**Social Food**:
- **Street Food**: Quick, cheap, eaten standing
- **Tavern Food**: Hearty, communal, social
- **Festival Food**: Special, expensive, ceremonial
- **Travel Rations**: Portable, preserved, bland

**Status Markers**:
- Poor eat: Gruel, hard bread, root vegetables
- Middle eat: Meat occasionally, fresh bread, ale
- Rich eat: Imported spices, wine, roasted meats

**Example (Coastal City)**:
- Staple: Fish stew with seaweed bread
- Special dish: Grilled ray-fin with lemon salt
- Street food: Fried fish cakes wrapped in kelp
- Status marker: Imported inland beef is luxury

Tag: `[LOCAL CUISINE: region X — staple: fish stew, special: grilled ray-fin, status marker: inland beef]`

---

## Clothing

What people wear signals status, profession, culture:

**Common Garments**:
- Base clothing everyone wears
- Seasonal variations
- Practical vs. ceremonial

**Status Markers**:
- **Poor**: Patched, worn, neutral colors, rough fabric
- **Middle**: Clean, fitted, some decoration, durable fabric
- **Rich**: Dyed colors, embroidery, jewelry, silk/velvet

**Professional Markers**:
- Blacksmith: Leather apron, burn marks
- Scholar: Ink-stained sleeves, reading glasses
- Soldier: Uniform elements even off-duty
- Merchant: Fine but practical, money pouch visible

**Cultural Markers**:
- Head coverings (religious, status, practical)
- Colors with meaning (mourning black, royal purple)
- Jewelry and adornment styles
- Taboo combinations (mixing faction colors, etc.)

**Example (Desert Nomads)**:
- Base: Loose robes, head wraps for sun protection
- Status: Quality of weave, silver jewelry
- Professional: Herders have striped patterns, warriors have red trim
- Taboo: Showing soles of feet is insulting

Tag: `[CLOTHING CODE: culture X — loose robes standard, red trim marks warriors, showing soles taboo]`

---

## Greetings and Social Protocol

How people interact in daily life:

**Greetings**:
- Formal: "I am honored to meet you, [title] [name]"
- Casual: "Well met, friend"
- Regional: "Good tide" (coastal), "Fair harvest" (farming)

**Physical Gestures**:
- Handshake? Bow? Hug? Kiss on cheek?
- Eye contact: Respectful or aggressive?
- Personal space: Close or distant?

**Address Titles**:
- How to address nobles, clergy, elders
- When to use first names vs. titles
- Insult by wrong form of address

**Example (Hierarchical City)**:
- Greeting: Lower status bows first, says "Your honor"
- Eye contact: Brief, then look down to show respect
- Address: Always use titles with superiors, first names with equals
- Insult: Address noble by first name without title → grave offense

Tag: `[SOCIAL PROTOCOL: culture X — bow to superiors, use titles always, first names insult]`

---

## Timekeeping

How do people mark the passage of time?

**Daily Time**:
- Sun position? Bell towers? Candle marks?
- "Meet at third bell" / "See you at high sun" / "Before the watch changes"

**Weekly/Monthly**:
- Market days? Holy days? Work cycles?
- "Every seventh day is rest day"

**Seasonal**:
- Named seasons: "Planting Time," "Long Dark," "Storm Season"
- Seasonal work: "During harvest" / "After first snow"

**Historical**:
- Years counted how? (From founding, from king's coronation, from divine event)
- "In the Year of Ash" / "Third year of Queen's reign" / "Ten winters ago"

**Example (Island Kingdom)**:
- Daily: Four tides per day, mark time by tide
- Weekly: Every fifth day is market gathering
- Seasonal: Monsoon Season, Calm Season, Storm Season
- Historical: Years since Great Wave (25 years ago)

Tag: `[TIMEKEEPING: culture X — four tides mark day, fifth day market, years since Great Wave]`

---

## Currency and Trade

What's used beyond standard gold pieces?

**Local Currency**:
- Coined money (standard)
- Metal weights (trade bars)
- Shells, beads, carved stones (regional)

**Barter System**:
- What goods commonly traded
- Standard exchanges: "One chicken = four loaves bread"
- When barter preferred over coin

**Status Currency**:
- **Favor**: "I owe you one" / "Three-favor debt"
- **Reputation**: "Good name is coin here"
- **Service**: "Work off the debt"

**Payment Terms**:
- Paid weekly? Daily? After job done?
- Deposits required? Penalties for late payment?

**Example (Mountain Dwarves)**:
- Standard: Coined gold and silver
- Premium: Mithral tokens for large trade
- Barter: Gemstones traded by carat weight
- Status: Craft-debt (owe a weapon, armor piece)

Tag: `[CURRENCY: culture X — gold coin standard, mithral tokens premium, craft-debt for status trades]`

---

## Festivals and Celebrations

Special days that break routine:

**Festival Elements**:
- **Name**: What's it called?
- **Timing**: When does it happen?
- **Purpose**: What's celebrated?
- **Activities**: Feasts, dancing, rituals, competitions?
- **Food/Drink**: Special dishes only for this day
- **Taboos**: What's forbidden during festival

**Festival Types**:
- **Seasonal**: Harvest Festival, First Snow Celebration
- **Religious**: Holy days, remembrance days
- **Historical**: Founding Day, Victory Anniversary
- **Life Cycle**: Coming of age, weddings, funerals

**Example (Coastal City — Tidecaller Festival)**:
- Timing: First day of Calm Season (when storms end)
- Purpose: Thank ocean for safe passage
- Activities: Boat races, seafood feast, offerings to sea
- Special food: Grilled fish with ceremonial spices
- Taboo: No fishing for three days after

Tag: `[FESTIVAL: location X — Tidecaller Festival, first Calm Season day, boat races and seafood feast]`

---

## Taboos and Superstitions

What's forbidden, unlucky, or offensive:

**Religious Taboos**:
- Desecrating temples
- Speaking god's true name
- Eating forbidden foods

**Social Taboos**:
- Insulting elders
- Breaking hospitality
- Touching sacred objects

**Superstitions**:
- Black cats, broken mirrors (universal)
- Local beliefs: "Never whistle at sea" / "Red sky means death"
- Lucky charms and warding gestures

**Consequences**:
- Minor: Social disapproval, bad luck
- Major: Exile, divine curse, execution

**Example (Nomadic Riders)**:
- Taboo: Never turn back on host's hearth (breaks hospitality)
- Superstition: Seeing white horse means journey blessed
- Consequence: Breaking hospitality → exile from all tribes

Tag: `[TABOO: culture X — never turn back on host's hearth, consequence: exile]`

---

## Marker Events

Events that everyone remembers and references:

**Historical Markers**:
- "The Great Fire" / "The Flood Year" / "When the Wall Fell"
- Everyone knows what you mean
- Used to date other events: "Two years after the Fire"

**Generational Markers**:
- Events older folk remember but young don't: "Before the War"
- Creates age-based information tiers

**Regional Markers**:
- Known in this region, unknown outside
- "You're not from here — you don't know about the Burning Summer"

Tag: `[MARKER EVENT: region X — The Great Fire, 15 years ago, everyone references]`

---

## Customs and Etiquette

Small rituals that signal membership:

**Hospitality Customs**:
- Guest offered food/drink first
- Shoes removed at door
- Host serves, then guest

**Trade Customs**:
- Shake hands to seal deal
- First offer always refused (polite)
- Written contracts vs. word-bond

**Conflict Customs**:
- Challenge to duel formally
- Apology requires specific words/gestures
- Mediator brought in for disputes

**Example (Mountain Clans)**:
- Hospitality: Guest drinks first, then host (proves not poisoned)
- Trade: First three offers refused as politeness, fourth is real
- Conflict: Blood-debt paid with service, not coin

Tag: `[CUSTOM: culture X — guest drinks first, three refusals polite, blood-debt paid by service]`

---

## Sensory Details

Texture comes alive through senses (see also [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md)):

**Smell**:
- Cooking food, smoke from fires
- Livestock, tanneries, breweries
- Flowers, incense, sea salt

**Sound**:
- Market calls, hammering, music
- Church bells, call to prayer, town criers
- Animals, weather, people talking

**Touch**:
- Rough cobblestones, smooth marble
- Hot sun, cold wind, humid air
- Fabric textures, wood grain, metal cool

Tag: `[SENSORY TEXTURE: location X — smell of grilled fish, sound of market calls, humid salt air]`

---

## Texture Across Social Class

Different texture for different classes:

**Lower Class**:
- Shared spaces, crowded
- Simple food, worn clothing
- Work-focused daily rhythm

**Middle Class**:
- Private homes, some space
- Varied diet, clean clothing
- Balance work and leisure

**Upper Class**:
- Estates, servants, privacy
- Imported luxuries, fashion
- Leisure-focused, social obligations

**Example texture variation**:
- Poor: Wake at dawn, eat gruel, work all day, sleep on straw
- Middle: Wake at sunrise, eat bread and cheese, work trade, sleep in bed
- Rich: Wake when ready, eat imported fruit, attend social events, silk sheets

Tag: `[CLASS TEXTURE: location X — lower class shares tenement rooms, middle class owns small homes, upper class has estates]`

---

## Seasonal Texture

How civilization changes with seasons:

**Work Changes**:
- Spring: Planting, building, travel resumes
- Summer: Harvests, festivals, long work days
- Autumn: Preparations for winter, markets busy
- Winter: Hunker down, indoor crafts, storytelling

**Food Changes**:
- Fresh vs. preserved foods
- Seasonal specialties
- Scarcity in lean seasons

**Mood Changes**:
- Spring: Optimistic, energetic
- Summer: Celebratory, social
- Autumn: Anxious, preparing
- Winter: Hunkered, introspective

Tag: `[SEASONAL TEXTURE: region X — spring planting frenzy, winter storytelling season, autumn anxiety]`

---

## Common Texture Mistakes

❌ **Medieval Europe default** — Not every fantasy world is medieval-ish
✅ **Distinctive culture** — Draw from varied Earth cultures, mix elements

❌ **No texture at all** — Just plot, no daily life
✅ **Sprinkle texture** — A few details per location make it real

❌ **Texture infodump** — Pages of cultural detail all at once
✅ **Reveal through play** — Show texture as PCs interact with world

❌ **All locations same texture** — Every village identical
✅ **Regional variation** — Different regions feel distinct

---

**See also:**
- [22-LOCATION-GENERATION.md](22-LOCATION-GENERATION.md) — Sensory registers for locations
- [25-REGION-GENERATION.md](25-REGION-GENERATION.md) — Civilization Texture Entry required
- [41-LINGUISTIC-SYSTEMS.md](41-LINGUISTIC-SYSTEMS.md) — Language as cultural marker
- [44-SOCIAL-SYSTEMS.md](44-SOCIAL-SYSTEMS.md) — Social networks and relationships
