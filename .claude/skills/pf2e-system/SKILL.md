---
name: pf2e-system
description: Pathfinder 2e system skill for working with PF2e mechanics, stat blocks, encounters, ancestries, items, spells, and rules in the Obsidian vault. Use when the user needs help with PF2e rules, monster creation, or mechanical content.
---

# Pathfinder 2e System Skill

This skill provides specialized instructions for working with Pathfinder 2e mechanics, stat blocks, encounters, and rules within the Obsidian vault.

## Folder Structure
When creating mechanical elements, place them in the appropriate subfolder within the `database/` directory, or in `pagine/` for general rules:
- `database/Personaggi/` (NPCs/Monsters with stat blocks)
- `database/Razze/` (Ancestries/Heritages)
- `database/Lignaggi/` (Versatile Heritages)
- `pagine/` (Rules, Mechanics, Items, Spells)

## Obsidian Features & Best Practices

### 1. Frontmatter (YAML)
Always include a comprehensive frontmatter block for mechanical entities to ensure they are easily queryable (e.g., via Dataview).

**Example for a Monster/NPC (`database/Personaggi/`):**
```yaml
---
aliases: [Monster Name]
tags: [monster, npc, level_X, trait_1, trait_2]
type: monster
level: 5
alignment: N
size: Medium
hp: 75
ac: 22
---
```

**Example for an Item/Spell (`pagine/`):**
```yaml
---
aliases: [Item Name]
tags: [item, consumable, level_X, magical]
type: item
level: 3
price: 10 gp
---
```

### 2. Stat Blocks (Markdown/Callouts)
Use Obsidian callouts or code blocks to format stat blocks clearly. If using a specific plugin (like TTRPG Statblocks), use its syntax. Otherwise, use standard markdown tables or callouts.

**Example Stat Block (Callout):**
```markdown
> [!statblock] Monster Name (Level 5)
> **Traits:** [Trait 1], [Trait 2]
> **Perception:** +12; Darkvision
> **Languages:** Common
> **Skills:** Athletics +14, Stealth +10
> **Str** +4, **Dex** +2, **Con** +3, **Int** -1, **Wis** +1, **Cha** +0
> ---
> **AC:** 22; **Fort:** +14, **Ref:** +11, **Will:** +10
> **HP:** 75
> ---
> **Speed:** 25 feet
> **Melee [1]** Strike Name +15 (agile, finesse), **Damage** 2d6+6 slashing
```

### 3. Linking Mechanics
- Always link to conditions, traits, and spells when referencing them (e.g., `[[Frightened]]`, `[[Fireball]]`).
- Use aliases for natural sentence flow: `[[Frightened|frightened 1]]`.

## Workflow
1. **Identify the Entity Type:** Determine if it's a monster, item, spell, or rule.
2. **Draft the Frontmatter:** Set up tags (including level and traits), aliases, and metadata.
3. **Format the Mechanics:** Use callouts or code blocks for clear, readable stat blocks.
4. **Link Extensively:** Ensure all mechanical terms (conditions, traits, spells) are linked to their respective notes.
