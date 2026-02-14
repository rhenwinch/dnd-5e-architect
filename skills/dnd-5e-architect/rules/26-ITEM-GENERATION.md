# 🗡️ ITEM & WEAPON GENERATION — Layer 6

**[LOAD PRIORITY: ON-DEMAND — Load when generating items, weapons, equipment, or treasure]**

---

## Layer 6 — Items, Weapons & Treasure

Items are not just statistics — they are story anchors, faction symbols, and player desire fulfillment tools. Every item should have clear mechanical value and meaningful world connections.

### Required Components

Every item must include:

- **Base Value** — The market price in gold pieces (MANDATORY)
- **Item Type** — Weapon, armor, consumable, tool, wondrous item, etc.
- **Rarity** — Common, Uncommon, Rare, Very Rare, Legendary, Artifact
- **Mechanical Effects** — What the item does in game terms (MANDATORY)
- **Faction or Creator Tie** — Who made this or controls its distribution?
- **Story Anchor** — Why does this item matter beyond its stats?
- **Acquisition Path** — How can players obtain this item?
- **Image Generation Prompt** (if enabled)

---

## MANDATORY: Item Value & Effects Rule

**ALL custom items and weapons MUST include:**

1. **Base Value (gp)** — The default market price
   - Cannot be "priceless" — use highest market tier (50,000+ gp) for truly rare items
   - Cannot be "variable" — provide a specific baseline price
   - Use standard D&D 5e pricing guidelines as reference
   
2. **Mechanical Effects** — Specific game mechanics
   - For weapons: damage dice, properties, attack bonus
   - For armor: AC bonus, disadvantage/advantage conditions
   - For magical items: spell effects, saving throw DCs, charges, recharge conditions
   - For consumables: duration, effect, limits
   - Cannot be "DM discretion" — provide baseline mechanics for DM to modify

**Rationale:** DMs need concrete starting points to adjudicate item balance, value, and trade. "Priceless" items break economy simulation. "DM discretion" creates prep burden.

Tag: `[ITEM MANDATORY: item X — Base Value: Y gp — Effect: Z]`

---

## Item Generation Template

```
## [Item Canonical Name]

**Item Type:** [Weapon / Armor / Wondrous Item / Consumable / Tool / Other]
**Rarity:** [Common / Uncommon / Rare / Very Rare / Legendary / Artifact]
**Base Value:** [X gp] — MANDATORY
**Attunement:** [Required / Not Required]

**MANDATORY: Mechanical Effects**
[Specific game mechanics — damage, AC, spell effects, bonuses, etc.]

Examples:
- Weapon: "1d8 slashing damage, finesse, light, +1 to attack and damage rolls"
- Armor: "AC 15 + Dex modifier (max 2), no disadvantage on Stealth"
- Wondrous: "Grants advantage on Charisma (Persuasion) checks when dealing with nobility"
- Consumable: "Drink as bonus action. Gain 2d4+2 temporary hit points for 1 hour"
- Magical: "Contains 3 charges. Expend 1 charge to cast Detect Magic. Regains 1d3 charges at dawn"

**Description:**
[Physical appearance, weight, materials, craftsmanship details]

**Faction or Creator Tie:** [Who made this? Who controls its distribution?]
- Is this item a faction signature? (uniforms, badges, weapons)
- Is this item faction-restricted? (guild tools, noble regalia, military gear)
- Who profits from this item's sale or use?
- Tag: `[FACTION TIE: item X — created/controlled/contested by faction Y]`

**Story Anchor:** [Why does this item matter beyond its stats?]
This should be something that:
- Connects to world history or lore
- Reveals faction dynamics or conflicts
- Creates player decision points
- Makes the item memorable

Examples:
- "This sword was forged from the chains of freed slaves — wearing it publicly is illegal in slaveholding nations"
- "This amulet bears the seal of the dissolved Mage Council — possessing it marks you as a target for the Empire"
- "This potion is brewed by a rival alchemist guild — buying it is an act of alliance"

**Acquisition Path:** [How can players obtain this item?]

Choose one or more:
- **Purchase**: Available at [location/merchant] for [price]
- **Commission**: Can be crafted by [NPC/faction] for [price + materials + time]
- **Quest Reward**: Granted by [NPC/faction] for [specific service]
- **Loot**: Found in [location] or dropped by [creature]
- **Theft**: Stealable from [location/NPC] with [risk]
- **Discovery**: Hidden in [location], requires [skill check or puzzle]

Tag: `[ACQUISITION: item X — method: Y — source: Z]`

**Consequence of Ownership:**
[What happens when players own or use this item?]
- Does owning this create faction reputation shifts?
- Does using this publicly attract attention?
- Does this item have enemies or admirers?
- Tag: `[CONSEQUENCE: item X owned — faction Y reacts with Z]`

**Image Generation Prompt:**
`[IMGPROMPT: ITEM — [description for visual generation]]`
```

---

## Item Rarity and Base Value Guidelines

Use these baseline prices as starting points:

| Rarity | Base Value Range | Example Items |
|---|---|---|
| **Common** | 25-100 gp | Standard weapons, basic tools, minor potions |
| **Uncommon** | 101-500 gp | +1 weapons/armor, useful wondrous items |
| **Rare** | 501-5,000 gp | +2 weapons/armor, powerful wondrous items |
| **Very Rare** | 5,001-50,000 gp | +3 weapons/armor, game-changing items |
| **Legendary** | 50,001-500,000 gp | Artifacts, unique faction treasures |
| **Artifact** | 500,000+ gp | World-shaping items, divine relics |

**Note:** Specific items may exceed or fall below these ranges based on context. The key is to provide a specific baseline price, not a range.

**For truly unique items:** Set base value at the highest tier for rarity level. DMs can rule "not for sale" but still need the value for theft, insurance, or consequence assessment.

Tag: `[ITEM VALUE: item X — rarity Y — base value Z gp]`

---

## Magical Item Effects Template

All magical items must specify:

### Passive Effects
[Always-on bonuses or properties]
- "+1 bonus to AC"
- "Advantage on saving throws against being frightened"
- "You can breathe underwater"

### Active Effects
[Requires action, bonus action, or reaction]
- **Activation Cost**: [action, bonus action, reaction, or triggered condition]
- **Effect**: [what happens mechanically]
- **Duration**: [instantaneous, 1 minute, 1 hour, until dispelled, etc.]
- **Limitation**: [uses per day, charges, cooldown, or condition]

### Charges (if applicable)
- **Total Charges**: [number]
- **Recharge**: [1d3 at dawn, all charges at dawn, never recharges, etc.]
- **Expend Charges**: [cost per effect]
- **Destruction Risk**: [if relevant — e.g., "If you expend the last charge, roll d20. On a 1, the item crumbles to dust"]

### Saving Throws & DCs (if applicable)
- **Save Type**: [Strength, Dexterity, Constitution, Intelligence, Wisdom, Charisma]
- **DC**: [specific number OR "spell save DC of attuned wielder"]
- **Success/Failure**: [what happens on each result]

**Example:**
```
## Shadowbrand Dagger

**Passive Effect:** +1 bonus to attack and damage rolls
**Active Effect (3 charges):**
- **Activation**: Bonus action after hitting with this weapon
- **Effect**: Target must succeed on a DC 13 Wisdom saving throw or become frightened of you for 1 minute
- **Duration**: 1 minute (target can repeat save at end of each turn)
- **Charges**: 3 total, regains 1d3 at dawn
```

---

## Item and Faction Integration

Items should not exist in a vacuum. They are created by, controlled by, or contested by factions.

**Questions to ask:**
- Which faction manufactures or controls this item?
- Which faction is trying to steal, ban, or monopolize this item?
- Which factions benefit or suffer from this item's existence?
- Is this item a faction symbol or identifier?

Tag faction ties: `[FACTION TIE: item X — relationship Y with faction Z]`

**Examples:**
- `[FACTION TIE: Guild Seal Ring — required by Merchant's Guild for legal trade]`
- `[FACTION TIE: Flame Tongue Sword — created by the Order of Eternal Fire, sought by the Dragon Cult]`
- `[FACTION TIE: Healing Potion — monopolized by the Alchemist Consortium, illegal to brew independently]`

---

## Item and Player Desire Integration

Items can serve as rewards for player desires:

| Player Desire | Item Reward Type |
|---|---|
| **Power** | Weapons, armor, ability-enhancing items |
| **Belonging** | Faction symbols, gifts from allies, heirlooms |
| **Revenge** | Tools to confront enemies, evidence items |
| **Knowledge** | Books, maps, Crystal balls, research tools |
| **Redemption** | Sacred relics, atonement tokens, guilt-linked items |
| **Wealth** | Gems, trade goods, valuable art, treasure |
| **Freedom** | Lock picks, escape tools, teleportation items |
| **Recognition** | Titles, medals, unique visible equipment |

Tag desire connections: `[DESIRE ANCHOR: item X — serves player desire Y via Z]`

See [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) for full Player Desire Matrix.

---

## Item Consequence Integration

Owning, using, or trading items should create ripples.

**If players purchase the item:**
- Merchant relationship established
- Faction benefits from gold flow
- Other factions may notice resources shift
- Tag: `[CONSEQUENCE: item X purchased — faction Y reacts with Z]`

**If players steal the item:**
- Original owner seeks return
- Fence or black market relationship needed
- Reputation as thief spreads
- Tag: `[CONSEQUENCE: item X stolen — faction Y pursues recovery]`

**If players use the item publicly:**
- Identifiable by signature magic or craftsmanship
- Factions react to visible power or symbol
- NPCs adjust behavior based on equipment
- Tag: `[CONSEQUENCE: item X used publicly — faction Y recognizes and reacts with Z]`

**If players sell or gift the item:**
- Item enters different hands
- New owner has own agenda
- Original owner may track item's location
- Tag: `[CONSEQUENCE: item X sold to NPC Y — new trajectory: Z]`

See [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) for consequence tracking.

---

## Legendary Items and Artifacts

Items of **Legendary** or **Artifact** rarity must include additional context:

### Origin Story
[Who created this item? Why? What was the cost?]

### Historical Impact
[What has this item done in the world? What events are tied to it?]

### Sentience (if applicable)
- **Intelligence/Wisdom/Charisma Scores**
- **Communication Method**: [telepathy, speech, empathic feelings]
- **Alignment**
- **Personality Traits**
- **Conflict Potential**: [what does the item want that might oppose the wielder?]

### Curse or Cost (optional but recommended)
[What price does the wielder pay for this power?]
- Mechanical penalties
- Obligation or quest imposed
- Transformation or corruption
- Tag: `[CURSED ITEM: item X — cost/curse: Y]`

### Destruction Condition
[How can this item be destroyed? Should it be destroyed?]
- Specific method only (e.g., "can only be destroyed in the volcano where it was forged")
- Moral cost of destruction (e.g., "destroying this releases the souls bound within")
- Tag: `[ARTIFACT DESTRUCTION: item X — method: Y — consequence: Z]`

---

## Common Item Generation Pitfalls

**Avoid:**
- Items with no base value ("priceless" or "variable")
- Items with no mechanical effects ("DM discretion")
- Items with no faction ties (who made this?)
- Items with no story relevance beyond stats
- Items that can't be obtained through player action
- Random loot with no world connection

**Prefer:**
- Items with specific baseline gold value
- Items with clear mechanical effects
- Items embedded in faction economies
- Items that create choices and consequences
- Items with multiple acquisition paths
- Items sourced from world systems

---

## Item Trading and Economy

When players attempt to sell items:

**Standard Items (Common/Uncommon):**
- Merchants buy at 50% base value
- Merchants sell at 100% base value
- Fences buy stolen goods at 25% base value

**Rare Items (Rare+):**
- Not all merchants can afford to purchase
- May require finding specialized buyer
- May attract unwanted attention
- Price negotiable based on buyer's wealth and desire

**Faction-Specific Items:**
- Original faction may pay premium for return (125-150%)
- Rival faction may pay premium for intelligence (150-200%)
- Selling to enemy faction creates reputation cost

Tag: `[ITEM TRADE: item X sold to NPC Y for Z gp — faction reaction: W]`

---

**See also:**
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction ties and resources
- [33-REWARD-SYSTEMS.md](33-REWARD-SYSTEMS.md) — Player Desire Matrix and reward types
- [32-CONSEQUENCE-SYSTEMS.md](32-CONSEQUENCE-SYSTEMS.md) — Item ownership consequences
- [51-IMAGE-GENERATION.md](51-IMAGE-GENERATION.md) — Visual generation for items
