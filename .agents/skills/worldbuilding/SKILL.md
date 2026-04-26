# Worldbuilding Skill

This skill provides specialized instructions for worldbuilding tasks within the Obsidian vault, focusing on creating rich lore, locations, NPCs, and factions.

## Folder Structure
When creating new worldbuilding elements, always place them in the appropriate subfolder within the `database/` directory:
- `database/Divinità/` (Deities)
- `database/Eventi/` (Events/History)
- `database/Fazioni/` (Factions/Organizations)
- `database/Insediamenti/` (Settlements)
- `database/Lignaggi/` (Lineages/Ancestries)
- `database/Lingue/` (Languages)
- `database/Luoghi/` (Locations/Geography)
- `database/Personaggi/` (NPCs/Characters)
- `database/Razze/` (Races/Species)

## Obsidian Features & Best Practices

### 1. Frontmatter (YAML)
Always include a comprehensive frontmatter block at the top of new files to ensure they are easily queryable (e.g., via Dataview).

**Example for an NPC (`database/Personaggi/`):**
```yaml
---
aliases: [Nickname, Title]
tags: [npc, faction_name, location_name]
type: npc
location: "[[City Name]]"
faction: "[[Faction Name]]"
status: alive
---
```

**Example for a Location (`database/Luoghi/` or `database/Insediamenti/`):**
```yaml
---
aliases: [Alternative Name]
tags: [location, settlement, region_name]
type: settlement
region: "[[Region Name]]"
population: 5000
ruler: "[[Ruler Name]]"
---
```

### 2. Linking and Backlinking
- Always use wikilinks (`[[Link]]`) to connect entities. If an entity doesn't exist yet, link it anyway to create a placeholder.
- Use aliases in links for natural sentence flow: `[[City Name|the bustling city]]`.
- Create "Relationships" or "Connections" sections at the bottom of notes to explicitly list related entities.

### 3. Templates
- Check the `_template/` folder for any existing templates before creating a new entity from scratch.
- If a template doesn't exist, structure the note logically with standard headings (e.g., for a Faction: `## Goals`, `## History`, `## Key Members`, `## Headquarters`).

## Workflow
1. **Identify the Entity Type:** Determine which `database/` subfolder the new entity belongs to.
2. **Draft the Frontmatter:** Set up tags, aliases, and metadata.
3. **Write the Content:** Focus on sensory details, motivations (for NPCs/Factions), and historical context.
4. **Link Extensively:** Ensure the new entity is woven into the existing world by linking to at least 2-3 other notes.
