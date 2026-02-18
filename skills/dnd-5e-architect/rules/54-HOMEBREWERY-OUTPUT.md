# 📜 HOMEBREWERY OUTPUT FORMAT

**[LOAD PRIORITY: OPTIONAL — Load when user chooses Homebrewery output format]**

---

## Overview

When the user selects **Homebrewery Markdown** as their output format, all generated `.md` files must follow [The Homebrewery](https://homebrewery.naturalcrit.com/) syntax instead of plain Markdown. Homebrewery Markdown is a superset of standard Markdown with custom class syntax, page breaks, column controls, and embedded CSS theming that renders as a styled PHB-like document.

**Reference:** See `references/homebrewery/phb-template.md` for a complete working example.

Tag: `[OUTPUT FORMAT: Homebrewery]`

---

## Mandatory File Header

Every Homebrewery output file MUST begin with two fenced code blocks in this exact order:

### 1. Metadata Block

````
```metadata
title: [Document Title]
description: [Brief description]
tags:
  - meta:Theme
systems:
  - 5e
renderer: V3
theme: 5ePHB
```
````

- **title:** Use the world/campaign name and document type (e.g., `Ashenmire — Factions`)
- **description:** Brief one-line summary
- **tags, systems, renderer, theme:** Always use the values shown above — do NOT change them

### 2. CSS Block

Immediately after the metadata block, include the **full CSS** from `references/homebrewery/phb-template.css` inside a fenced `css` code block. Copy the CSS **verbatim** — do not modify, minify, or omit any part of it.

````
```css
/* Paste the ENTIRE contents of references/homebrewery/phb-template.css here */
/* Do NOT modify the CSS in any way */
```
````

**Why:** The CSS provides the custom PHB 2024 theme styling (fonts, colors, borders, stat blocks, page textures). Altering it breaks visual consistency.

---

## Page Structure

### Page Breaks

Use `\page` on its own line to create a new page:

```
Content on page 1...

\page

Content on page 2...
```

### Column Breaks

Use `\column` on its own line to force a column break within a two-column page:

```
Left column content...

\column

Right column content...
```

Standard content pages are **two-column** by default. Special pages (covers, full-page art, wide TOC) override this.

---

## Page Types

Homebrewery uses **class markers** with double-curly-brace syntax `{{className}}` to designate page types. Place the class marker at the **top** of the page content (after `\page`).

### Front Cover

```
{{frontCover}}

### [SUBTITLE TEXT]

## [SERIES OR BRANDING]

# [Main Title]

![Front Cover Image](image-url) {bottom:-7.4%,left:-416px,height:115%}
```

### Inside Cover

```
{{insideCover}}

# [Title]
___
{width:10cm}

![background image](image-url){position:absolute,top:295px,left:175px,width:465px}

{{watercolor6,top:0px,left:830px,width:320px,transform:rotate(-50deg),background-color:#aaa4bc,opacity:70%}}

{{artist,left:38px
[Artist Name](artist-url)
}}

{{logo ![](/assets/naturalCritLogoRed.svg)}}
```

### Back Cover

```
{{--height:708px

{{backCover}}

![background image](image-url){}

# [Title]

[Back cover description text...]

{{banner
A companion to [other documents or links]
}}

{{logo
![Logo](logo-url)

[Branding Text]
___

[URL](url)
}}

}}
```

### Credits Page

```
{{credits}}

# Credits

**[Role]:** :: [Name/Link]

##### [Credit Section]
**[Item]:** :: [Credit details]
```

The `::` separator creates hanging-indent definition lists used for credit formatting.

### Table of Contents

```
{{toc,wide
# Contents

- ### [{{ Section Title}}{{ page#}}](#pN)
  - #### [{{ Subsection}}{{ page#}}](#pN)
    -  [{{ Sub-subsection}}{{ page#}}](#pN)
}}
```

- The `wide` class makes the TOC span **3 columns**
- Use `{{ Title}}{{ page}}` format inside links
- Anchor targets use `#pN` where N is the page number
- Omit `wide` for a standard 2-column TOC

### Full-Page Art

```
{{fullPage

![image](image-url) {width:950px,left:-45px;}

}}

{{caption,right
Caption text describing the scene
}}

# [Page Title]

{{banner,--color:"rgba(177, 154, 120, 0.8)"
## [Banner Subtitle]
}}

{{artist
[Artist Name](artist-url)
}}
```

### Chapter Header

```
{{chapter,gradient,--color:#7c4848

## [chapter number]
# [Chapter Title]
___
}}
```

**Gradient color values** (approximate PHB chapter colors for reference):
| Color Hex | Usage |
|---|---|
| `#b39a59` | Intro / Index (Yellow) |
| `#9a4835` | Chapter-style (Pink-red) |
| `#676b36` | Chapter-style (Green) |
| `#a74d3a` | Chapter-style (Red-Orange) |
| `#8a86b2` | Chapter-style (Light Blue) |
| `#7c4848` | Chapter-style (Dark Red) |
| `#5fa7a1` | Chapter-style (Cyan) |
| `#9a677b` | Chapter-style (Mauve) |

- Add `noCap` to disable the drop-cap on the first paragraph: `{{chapter,gradient,noCap,--color:#hex}}`
- Omit `gradient` for a chapter header without the gradient background

---

## Content Elements

### Notes (Callout Boxes)

```
{{note
##### Note Title
Note content here. Styled with beige/parchment background.
}}
```

### Descriptive Text (Read-Aloud Boxes)

```
{{descriptive
**Label.** :: Description text here.
Styled with blue-tinted border — use for read-aloud or boxed text.
}}
```

### Monster Stat Blocks (2024 Style)

Single-column stat block:

```
{{monster,frame
## [Monster Name]
*[Size] [Type], [alignment]*

**AC**         :: [value] ([armor source])
**HP**         :: [value] ([dice formula])
**Speed**      :: [value]

**Initiative** :: +[mod] ([score])

|   |   | MOD | SAVE |   |   | MOD | SAVE |   |   | MOD | SAVE |
|:--|:-:|:---:|:----:|:--|:-:|:---:|:----:|:--|:-:|:---:|:----:|
|Str| [score]| +[mod] | +[save] |Dex| [score]| +[mod] | +[save] |Con| [score]| +[mod] | +[save] |
|Int| [score]| +[mod] | +[save] |Wis| [score]| +[mod] | +[save] |Cha| [score]| +[mod] | +[save] |

**Immunities**  :: [list]
**Senses**      :: [list]
**Languages**   :: [list]
**CR**          :: [value] (XP [xp]; PB +[pb])

### Traits
***[Trait Name].*** [Description]

### Actions
***[Action Name].*** *[Attack Type]:* +[hit], reach [X] ft. *Hit:* [damage] ([dice] + [mod]) [type] damage.

### Legendary Actions
{{legend Legendary Action Uses: [N]. [Recharge description].}}

***[Action Name].*** [Description]

}}
```

For wide (two-column) stat blocks, use `{{monster,frame,wide}}`.

**Note:** Use `--` (double dash) for negative modifiers in the ability table (e.g., `--1` for -1).

### Spell Lists

```
{{spellList}}

##### [Spell Level] Spells
| Spell | School | Special |
|:------|:-------|:-------:|
| *[Spell Name]* | [School] | [C/R/M/—] |
```

The `{{spellList}}` class ensures uniform first-column widths across all tables on the page.

### Class Feature Tables

```
{{classSymbol ![](symbol-url) {width:40px,margin-top:5px} }}

{{classTraits
##### Core [Class] Traits
| | |
|:------|:------|
| **Primary Ability** | [Ability] |
| **Hit Point Die** | [Die] per [Class] level |
| ... | ... |
}}
```

### Origin / Background Headers

```
{{origin,--height:330px
![background art](image-url){}
}}

### [Origin Name]
**Ability Scores:**       :: [list]
**Feat:**                 :: [feat]
**Skill Proficiencies:**  :: [list]
**Tool Proficiency:**     :: [tool]
**Equipment:**            :: [list]
```

The `--height` variable controls the image height. Subsequent origins on the same page automatically get a gold separator line.

---

## Layout & Formatting Elements

### Page Numbers & Footnotes

Place at the **bottom** of each content page:

```
{{pageNumber,auto}}
{{footnote Chapter X | Section Title}}
```

- `auto` auto-increments the page number
- Replace `auto` with a specific number for manual control
- The `.light` class changes color to gold: `{{pageNumber.light,auto}}`

### Artist Credits

```
{{artist
[Artist Name](artist-url)
}}
```

Renders as rotated text on the left edge of the page. Add `,bottom:Npx` to control vertical position:

```
{{artist,bottom:630px [Artist Name](url)}}
```

### Captions

```
{{caption
Caption text here
}}
```

- Add `right` for right-side placement: `{{caption,right}}`
- On half-page images, use `rightCaption` instead: `{{caption,rightCaption}}`

### Horizontal Rules

```
___
```

Three underscores create the gray horizontal separator bar.

### Vertical Spacing

```
::
```

A single `::` on its own line creates a small vertical spacer. Multiple `::` lines add more space.

### Small Caps

```
<caps>Dungeons & Dragons</caps>
```

Use for trademarked terms or stylistic small-caps text.

### The Spacer Class

```
{{spacer}}
```

Creates a tiny vertical space — smaller than `::`.

### Banners

```
{{banner,--color:"rgba(177, 154, 120, 0.8)"
## Banner Text
}}
```

### Definition Lists (Hanging Indent)

```
**Label:** :: Value text
```

The `::` separator creates a hanging-indent definition list entry.

---

## Image Handling

### Conditional Image Inclusion

**IMPORTANT:** Only include images in Homebrewery output if the campaign/world has generated images available at:

```
[campaign-name]/images/**/*.[png|jpg|jpeg|webp|svg]
```

If the images directory is **empty or does not exist**, omit ALL image elements (front covers, full-page art, half-page art, origin headers, watercolor stains, etc.). The document should still function correctly without images — the text content and structure remain intact.

When images ARE available, reference them using relative paths from the document location.

### Inline Image Styling

Homebrewery supports inline CSS on images using curly braces:

```
![alt text](url) {position:absolute,top:100px,left:50px,width:300px}
```

Common properties: `position`, `top`, `left`, `right`, `bottom`, `width`, `height`, `z-index`, `min-width`, `min-height`, `transform`

### Half-Page Bordered Images

```
{{imageWrapper,--maskWidth:332px,--maskHeight:1048px,--maskLeft:41px,--maskTop:29px

{{borderImage ![alt](image-url) {top:0px,left:0px} }}

{{caption,rightCaption
Caption text
}}

}}
```

Use `leftSide` or `rightSide` shortcuts for full-height half-page images:

```
{{imageWrapper.leftSide
{{borderImage ![alt](url) {top:0px,left:0px} }}
}}
```

### Watercolor Stains

```
{{watercolor6,top:0px,left:830px,width:320px,transform:rotate(-50deg),background-color:#aaa4bc,opacity:70%}}
```

12 variants available: `watercolor1` through `watercolor12`.

---

## Homebrewery Document Structure Template

When generating a **complete world document** or **campaign module** in Homebrewery format, follow this page order:

### For World Documents

```
Page 1:  [metadata + CSS] + Front Cover (if images exist)
Page 2:  Inside Cover (if images exist) OR Title + Credits
Page 3:  Credits (if not on page 2)
Page 4:  Table of Contents
Page 5+: Content pages (chapter headers + body text)
Last:    Back Cover (optional, if images exist)
```

### For Campaign Session Modules

```
Page 1:  [metadata + CSS] + Module Header (campaign name, session #, title)
Page 2:  Table of Contents
Page 3+: Module content (parts, encounters, NPC guides, etc.)
```

### If No Images Available

```
Page 1:  [metadata + CSS] + Title Page (chapter header style, no cover art)
Page 2:  Table of Contents
Page 3+: Content pages
```

---

## Plain Markdown ↔ Homebrewery Mapping

When converting existing plain Markdown content to Homebrewery format, apply these translations:

| Plain Markdown | Homebrewery Equivalent |
|---|---|
| `# Title` | Chapter header: `{{chapter,gradient,...}} # Title` |
| `## Section` | `## Section` (unchanged — rendered with PHB styling) |
| `### Subsection` | `### Subsection` (gold underline from CSS) |
| `> blockquote` (DM secret) | `{{note}} ... {{}}` or keep as blockquote |
| Horizontal rule `---` | `___` (three underscores) |
| Standard table | Standard table (CSS styles it automatically) |
| Monster stat block (plain) | `{{monster,frame}} ... {{}}` |
| Read-aloud text | `{{descriptive}} ... {{}}` |
| Page/section break | `\page` |
| File metadata header | ````metadata``` + ```css``` blocks |

---

## Quality Checklist

Before delivering a Homebrewery document, verify:

- [ ] Metadata block is first, with correct renderer (`V3`) and theme (`5ePHB`)
- [ ] Full CSS from `references/homebrewery/phb-template.css` is included verbatim
- [ ] Every page after the first has `\page` separator
- [ ] Content pages have `{{pageNumber,auto}}` and `{{footnote ...}}`
- [ ] Monster stat blocks use `{{monster,frame}}` syntax
- [ ] Read-aloud text uses `{{descriptive}}` blocks
- [ ] Notes use `{{note}}` blocks
- [ ] Chapter transitions use `{{chapter,gradient,--color:#hex}}` with `___` separator
- [ ] Images are only included if `[campaign-name]/images/` contains files
- [ ] Two-column layout is maintained (use `\column` for manual breaks)
- [ ] `::` definition list syntax used for labeled fields (AC, HP, Speed, etc.)
- [ ] No plain Markdown horizontal rules (`---`) — use `___` instead

---

**See also:**
- [04-CORE-OUTPUT-FORMAT.md](04-CORE-OUTPUT-FORMAT.md) — Output format selection and plain Markdown rules
- [10-SESSION-INITIALIZATION.md](10-SESSION-INITIALIZATION.md) — Where the format preference is gathered
- `references/homebrewery/phb-template.md` — Complete working reference document
- `references/homebrewery/phb-template.css` — PHB 2024 custom theme CSS (include verbatim)
