# Creative Storytelling Skill

This skill provides specialized instructions for crafting narrative arcs, plot hooks, character development, themes, and descriptions within the Obsidian vault.

## Folder Structure
When brainstorming or drafting narrative elements, place them in the appropriate subfolder:
- `bozze/` (Drafts, brainstorming, unrefined ideas)
- `sessioni/` (For session-specific narrative beats)
- `database/Personaggi/` (For character arcs and motivations)
- `database/Eventi/` (For historical narratives)

## Obsidian Features & Best Practices

### 1. Frontmatter (YAML)
Always include a comprehensive frontmatter block for narrative drafts to track their status and themes.

**Example for a Narrative Draft (`bozze/`):**
```yaml
---
aliases: [Draft Title]
tags: [draft, narrative, theme_name, character_arc]
type: narrative
status: brainstorming
related_characters: ["[[Character 1]]", "[[Character 2]]"]
---
```

### 2. Narrative Structure & Themes
Use a consistent structure for narrative drafts. Focus on themes, conflicts, and character arcs.

```markdown
# [Narrative Arc Title]

## Core Theme
- What is the central theme of this arc? (e.g., Betrayal, Redemption, Discovery)

## Key Conflicts
- **Internal:** What is the character struggling with internally?
- **External:** What external forces are opposing the character?

## Plot Beats
1. **Inciting Incident:** What kicks off the arc?
2. **Rising Action:** Key events that escalate the conflict.
3. **Climax:** The peak of the conflict.
4. **Resolution:** How does the arc conclude?

## Character Arcs
- **[[Character 1]]:** How do they change from the beginning to the end?
- **[[Character 2]]:** What is their role in the arc?
```

### 3. Linking and Backlinking
- Link themes to specific characters, locations, or events.
- Use aliases for natural sentence flow: `[[Theme Name|the underlying theme]]`.
- Create "Connections" sections to explicitly link narrative arcs to specific sessions or worldbuilding elements.

### 4. Canvas (Obsidian Feature)
If using Obsidian Canvas, use it to visually map out complex narrative webs, character relationships, or timeline events. Link nodes in the canvas back to the detailed markdown notes in `bozze/` or `database/`.

## Workflow
1. **Brainstorm in `bozze/`:** Start with rough ideas, themes, and conflicts.
2. **Draft the Frontmatter:** Set up tags, status, and related characters.
3. **Structure the Narrative:** Use the standard structure (Theme, Conflicts, Plot Beats, Character Arcs).
4. **Link Extensively:** Ensure all narrative elements (characters, locations, themes) are linked to their respective notes in the `database/` or `sessioni/` folders.
5. **Refine and Move:** Once a draft is finalized and ready to be implemented in a session, integrate its elements into the appropriate `sessioni/` prep notes or update the relevant `database/` entries.
