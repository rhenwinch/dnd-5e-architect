# 🗣️ LINGUISTIC SYSTEMS

**[LOAD PRIORITY: ENHANCEMENT — Load when adding language detail, dialects, or speech patterns]**

---

## Why Language Matters

Language distinguishes:
- **Social class** (formal vs. colloquial)
- **Regional identity** (accents, local terms)
- **Faction membership** (jargon, shibboleths)
- **NPC personality** (speech patterns make NPCs memorable)
- **Cultural texture** (how people talk shapes how the world feels)

---

## Voice Register System

Every location, faction, and NPC should have a declared **Voice Register** — the formality and style of speech.

### The Six Voice Registers

| Register | Description | Examples |
|---|---|---|
| **Formal** | Precise, elevated, structured | Courts, temples, academic institutions |
| **Colloquial** | Casual, everyday, relaxed | Taverns, markets, homes |
| **Mythic** | Ancient, grand, timeless | Gods, cosmic entities, ancient texts |
| **Predatory** | Threatening, commanding, sharp | Villains, military commanders, crime lords |
| **Haunted** | Fractured, hesitant, broken | Traumatized NPCs, cursed locations, decay |
| **Technical** | Specialized, precise, jargon-heavy | Guilds, craftspeople, scholars |

Tag: `[VOICE REGISTER: element X — register: Formal/Colloquial/Mythic/Predatory/Haunted/Technical]`

---

## Speech Register (for NPCs)

NPCs need specific speech patterns that make them memorable and distinct.

### Format

```
**Speech Register:**
- **Formality**: [High / Medium / Low]
- **Distinctive Patterns**: [specific verbal habits]
- **Vocabulary**: [specialized terms, favorite phrases]
- **Tells**: [speech changes when lying, nervous, angry]

Tag: [SPEECH REGISTER: NPC X — pattern: Y]
```

### Examples

**Formal Speech**:
- "I am pleased to make your acquaintance"
- Never uses contractions
- Addresses people by title
- Complete sentences, proper grammar

**Colloquial Speech**:
- "Nice to meetcha"
- Heavy use of contractions
- Casual pronouns
- Sentence fragments, slang

**Technical Speech**:
- "The tensile strength of the alloy exceeds standard parameters"
- Guild-specific jargon
- Precision over clarity
- Assumes listener shares knowledge

---

## Linguistic Profile (for Regions and Factions)

Regions and factions should have linguistic profiles that distinguish them.

### Format

```
**Linguistic Profile:**
- **Primary Language(s)**: [what languages spoken here]
- **Formality Level**: [High / Medium / Low]
- **Distinctive Vocabulary**: [regional terms, slang, idioms]
- **Accent/Dialect Notes**: [pronunciation quirks, grammar patterns]
- **Code-Switching**: [do people change language/register based on context?]

Tag: [LINGUISTIC PROFILE: element X — primary language: Y — formality: Z]
```

### Examples

**Urban Merchant District**:
- Primary: Common, with Trade Pidgin for merchants
- Formality: Medium to High (business professional)
- Vocabulary: "Fair coin" (good deal), "copper-clutcher" (cheapskate)
- Accent: Crisp consonants, dropped H's
- Code-Switching: Formal with customers, colloquial with fellow merchants

**Rural Farming Region**:
- Primary: Common, regional dialect
- Formality: Low (casual, friendly)
- Vocabulary: "First-frost" (autumn), "mudtime" (spring), "harvestgold" (payment)
- Accent: Drawled vowels, soft R's
- Code-Switching: More formal with outsiders, dialect with locals

---

## Dialect Markers

Create distinctive dialects without being offensive or cartoonish:

### Phonetic Markers (pronunciation)
- Dropped consonants: "goin'" instead of "going"
- Added sounds: "arsk" instead of "ask"
- Vowel shifts: "git" instead of "get"

### Grammatical Markers
- Word order changes: "Going to market, I am"
- Double negatives: "I don't know nothing"
- Different verb forms: "We was going" / "They goes there"

### Vocabulary Markers
- Regional terms for common items
- Unique idioms and expressions
- Borrowed words from other languages

**Use sparingly** — one or two markers per dialect is enough.

Tag: `[DIALECT: region X — marker: dropped final consonants in -ing words]`

---

## Shibboleths and Code Words

Factions use language to identify members:

**Shibboleth**: A word or phrase that's difficult for outsiders to pronounce or know
- "The Archive keeps what password?" "The copper remembers"
- Only members know the response

**Jargon**: Specialized terms that signal membership
- Thieves' cant for criminal organizations
- Guild technical terms for craftspeople
- Military slang for soldiers

**Formality Shifts**: Using wrong register signals outsider status
- Address a crime lord with formal court language → immediately marked as outsider
- Use casual slang with a noble → disrespect or ignorance

Tag: `[FACTION LANGUAGE: faction X — shibboleth: Y — jargon: Z]`

---

## Voice Register Collision

When characters from different registers interact, create interesting tension:

**Examples**:
- Formal scholar tries to negotiate with Colloquial street gang (miscommunication)
- Colloquial hero meets Mythic god (awe and inadequacy)
- Predatory villain taunts Haunted victim (power dynamic visible through speech)

Tag: `[VOICE REGISTER COLLISION: NPC A (Formal) meets NPC B (Colloquial) — tension: miscommunication]`

---

## Code-Switching

People change how they speak based on context:

**Social Code-Switching**:
- Formal with superiors, Colloquial with peers
- Technical with colleagues, simplified with outsiders
- Regional dialect at home, Standard Common in city

**Strategic Code-Switching**:
- NPC pretends to be lower class (speaks Colloquial to blend in)
- Faction member signals membership (drops into jargon)
- Character intimidates (shifts to Predatory register)

Tag: `[CODE-SWITCHING: NPC X shifts from Formal to Colloquial when among friends]`

---

## Multilingualism

In diverse settings, track who speaks what:

**Common Patterns**:
- **Trade Common**: Everyone speaks some
- **Regional Languages**: Native speakers plus neighbors
- **Rare Languages**: Scholars, spies, specific factions
- **Dead Languages**: Scholars only, or ancient texts

**Language as Barrier**:
- PC doesn't speak local dialect → needs translator
- Secret conversation in language PCs don't know
- Ancient text requires specific knowledge to read

**Language as Key**:
- Password must be spoken in specific language
- Ritual requires ancient tongue
- Treaty valid only in language it was written

Tag: `[LANGUAGE BARRIER: location X — primary language: Y — Common speakers: rare]`

---

## Speech Patterns for Memorable NPCs

Make NPCs memorable through distinctive speech:

**Verbal Tics**:
- Repeats words: "The thing, the thing is..."
- Filler words: "You see," "As it were," "Y'know"
- Unusual syntax: "Powerful, you are" (Yoda-style)

**Emotional Tells**:
- Laughs nervously before lying
- Formal language when anxious
- Stutters when angry
- Goes silent when sad

**Thematic Patterns**:
- Speaks in metaphors: "Life is a river, friend"
- Uses nautical terms: "All hands on deck"
- Quotes proverbs: "As my grandmother said..."

Tag: `[SPEECH PATTERN: NPC X — laughs nervously before revealing secrets]`

---

## Linguistic Texture vs. Readability

**Balance detail with clarity**:

❌ **Too much** — "Ah, yer lookin' fer th' Archive, eh? Aye, 'tis three blocks hence, past th' ol' smithy, d'ye ken?"
✅ **Just enough** — "You're looking for the Archive? Aye, it's three blocks east, past the old smithy, you understand?"

**Write phonetically sparingly**:
- One or two markers per character
- Avoid wall-of-apostrophes
- Describe speech patterns in Roleplaying Notes instead

**Example**:
Instead of writing heavy dialect, write:
> **Roleplaying Notes**: Old Tam speaks in a thick rural dialect, dropping final consonants and using farming metaphors. Players hear "harvestgold" for payment, "first-frost" for autumn.

Then write dialogue normally with those terms inserted.

---

## Speech and Information Tier

How someone talks can reveal information:

**Accent reveals origin**:
- "That's a northern accent — you're from the mountains"
- NPCs familiar with region can identify outsiders

**Formality reveals class**:
- Formal speech → educated, possibly noble
- Colloquial speech → working class, possibly rural

**Slang reveals affiliation**:
- Uses thieves' cant → likely criminal
- Uses military jargon → veteran or soldier
- Uses archaic terms → scholar or ancient being

Tag: `[LINGUISTIC TELL: NPC X accent reveals southern origin — Information Tier: PUBLIC]`

---

## Common Linguistic Mistakes to Avoid

❌ **Every NPC sounds the same** — Vary registers and patterns
✅ **Distinctive voices** — Each NPC has unique speech

❌ **Unreadable phonetic spelling** — "Ah canna understan' wha' yer sayin'"
✅ **Readable with markers** — Describe accent, use a few key terms

❌ **Offensive stereotypes** — Real-world ethnic stereotypes
✅ **Fantasy-specific patterns** — Create new linguistic cultures

❌ **Inconsistent speech** — NPC formal one scene, colloquial the next (without reason)
✅ **Consistent register** — Speech changes only with code-switching or emotional state

---

**See also:**
- [20-NPC-GENERATION.md](20-NPC-GENERATION.md) — Speech Register for NPCs
- [21-FACTION-GENERATION.md](21-FACTION-GENERATION.md) — Faction Linguistic Profile
- [25-REGION-GENERATION.md](25-REGION-GENERATION.md) — Regional Linguistic Profile
- [42-CIVILIZATION-TEXTURE.md](42-CIVILIZATION-TEXTURE.md) — Language in daily life
