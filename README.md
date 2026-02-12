# DND 5e Architect - Agent Skill

A modular D&D 5e worldbuilding system packaged as a GitHub Copilot Agent Skill.

## What is This?

This is an Agent Skill for GitHub Copilot that teaches the AI how to generate rich, interconnected D&D 5e worlds, campaigns, NPCs, factions, locations, and more.

## Installation

This skill is a **project skill** and will automatically be available to Copilot when working in this repository.

To use this skill in your own projects:

1. Copy the `.github/skills/dnd-5e-architect/` directory to your project
2. GitHub Copilot will automatically detect and use it when relevant

For personal use across all projects, copy to `~/.copilot/skills/dnd-5e-architect/` or `~/.claude/skills/dnd-5e-architect/`.

## How It Works

The skill contains 32 modular instruction files organized by priority:

- **CORE (01-05)**: Always loaded - identity, philosophy, consistency, output format, safety rules
- **STARTUP (10)**: Mode detection and initialization
- **ON-DEMAND (20-25)**: Element-specific generation (NPCs, factions, locations, creatures, regions)
- **CROSS-SYSTEM (30-34)**: Special mechanics (information, time, consequences, rewards, morality)
- **ENHANCEMENT (40-44)**: Optional depth (spatial, linguistic, civilization, emotional, social)
- **SPECIAL (50-51)**: Combat and image generation
- **MAINTENANCE (60-61, 70-71, 80)**: Audits, formats, compression
- **REFERENCE (00, 90-91)**: Backup and glossary

## Features

### Two Operational Modes

**World Building Mode (Default)**
- Creates standalone, reusable worlds
- No player assumptions
- Supports multiple campaigns

**Campaign Mode** 
- Integrates with active players
- Session-to-session tracking
- Player-specific consequences

### File Organization

Outputs are organized in a clean directory structure:

```
worlds/
└── [world-name]/
    ├── [world-name]-readme.md
    ├── [world-name]-factions.md
    ├── [world-name]-npcs.md
    └── campaigns/
        └── [campaign-name]/
            ├── [campaign-name]-readme.md
            └── [campaign-name]-session-log.md
```

### Key Principles

1. **Four Laws of Interconnection**: Every element must satisfy Causality, Conflict, Secrecy, and Fragility
2. **Plot Web**: Visual connections between elements
3. **Living Clock**: World progresses independently
4. **Modular Loading**: Load only what you need (50-85% token savings)

## Usage Examples

Once installed, simply ask Copilot:

- "Build a dark fantasy world with three warring factions"
- "Generate 5 NPCs for a noir fantasy city"
- "Create a complete region with locations and conflicts"
- "Start a campaign in an existing world"
- "Design a lich villain with layers of secrecy"

Copilot will automatically use this skill and follow the modular instruction system.

## Documentation

See [SKILL.md](.github/skills/dnd-5e-architect/SKILL.md) for complete documentation on:
- When to use which files
- Modular loading patterns
- Output requirements
- Mode detection logic

## License

MIT

## About Agent Skills

Agent Skills are folders of instructions and resources that enhance GitHub Copilot's abilities in specialized domains. Learn more at the [Agent Skills standard](https://github.com/agentskills/agentskills).
