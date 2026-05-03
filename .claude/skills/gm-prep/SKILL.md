---
name: gm-prep
description: Game Master prep skill for preparing TTRPG sessions, designing encounters, managing loot, and writing session recaps in the Obsidian vault. Use when the user wants to plan, prep, or recap a session.
---

# Game Master Prep Work Skill

This skill provides specialized instructions for preparing TTRPG sessions, designing encounters, managing loot, and writing recaps within the Obsidian vault.

## Folder Structure
When preparing for a session, always place your notes in the appropriate subfolder within the `sessioni/` directory:
- `sessioni/` (Session notes, recaps, prep work)
- `sessioni/Ambizioni Sommerse/` (Campaign-specific session notes)
- `_template/` (Templates for session prep, NPCs, encounters)

## Obsidian Features & Best Practices

### 1. Frontmatter (YAML)
Always include a comprehensive frontmatter block for session notes to ensure they are easily queryable (e.g., via Dataview) and organized chronologically.

**Example for a Session Note (`sessioni/Ambizioni Sommerse/`):**
```yaml
---
aliases: [Session X]
tags: [session, prep, recap, campaign_name]
type: session
session_number: 1
date: 2024-05-01
status: prepped
---
```

### 2. Session Prep Structure
Use a consistent structure for session prep notes. If a template exists in `_template/`, use it. Otherwise, structure the note logically:

```markdown
# Session X: [Title]

## Recap
- Brief summary of the previous session.

## Objectives / Hooks
- What are the players trying to achieve?
- What hooks are available?

## Scenes / Encounters
### Scene 1: [Name]
- **Location:** `[[Location Name]]`
- **NPCs:** `[[NPC 1]]`, `[[NPC 2]]`
- **Description:** Sensory details and initial situation.
- **Encounter:** `[[Monster 1]]` (x2), `[[Hazard 1]]`
- **Loot:** `[[Item 1]]`, 50 gp

### Scene 2: [Name]
...

## Secrets & Clues
- [ ] Clue 1 (Points to `[[Location/NPC]]`)
- [ ] Clue 2 (Reveals `[[Lore/Secret]]`)

## Post-Session Notes
- What actually happened?
- What needs to be prepped for next time?
```

### 3. Linking and Backlinking
- Always link to locations, NPCs, monsters, and items referenced in the prep.
- Use aliases for natural sentence flow: `[[City Name|the bustling city]]`.
- Link back to previous sessions if referencing past events.

## Workflow
1. **Create the Session Note:** Place it in the correct campaign folder under `sessioni/`.
2. **Draft the Frontmatter:** Set up tags, session number, date, and status.
3. **Structure the Prep:** Use a template or the standard structure (Recap, Objectives, Scenes, Secrets).
4. **Link Extensively:** Ensure all entities (NPCs, locations, monsters, items) are linked to their respective notes in the `database/` or `pagine/` folders.
5. **Update Post-Session:** After the session, update the note with what actually happened and change the status to `played`.
