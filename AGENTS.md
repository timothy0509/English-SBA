# AGENTS.md

## Repository Type

Obsidian markdown knowledge base for an English School-Based Assessment (SBA). No build system, package manager, or tests — edits are purely to Markdown content.

## Workspace Conventions

- **Vault root**: `Five People You Meet in Heaven/`
- **Link syntax**: Wikilinks `[[Note Name]]` and aliased wikilinks `[[Note Name|Display Text]]`
- **Frontmatter**: Every note has YAML frontmatter with `title`, `description` (optional), and `tags`
- **Index notes**: Numbered `00 - Home.md` through `07 - Exam Oral Prep.md` serve as entrypoints and maps of content (MOCs)
- **Entity notes**: Character, theme, and lesson notes use title-case names (e.g. `Eddie.md`, `Theme - Connection.md`, `Lesson 1 - Connection.md`)

## File Organization

```
Five People You Meet in Heaven/
  00 - Home.md              # Entrypoint / navigation hub
  01 - Book Overview.md
  02 - Characters MOC.md    # Links to all character notes
  03 - The Five Lessons MOC.md
  04 - Plot Timeline.md
  05 - Key Quotes.md
  06 - Study Guide.md
  07 - Exam Oral Prep.md
  Eddie.md, Marguerite.md, ...   # Character notes
  Theme - *.md                    # Theme notes
  Lesson 1 - Connection.md, ...   # Lesson notes
```

## Gotchas

- `.obsidian/workspace.json` is gitignored ( Obsidian auto-generates it ), but other `.obsidian/` files are tracked. Do not manually add `workspace.json`.
- When renaming a note, update all wikilinks that point to it. Obsidian does this automatically if opened in Obsidian, but in raw file edits it is manual.
- Callout blocks use Obsidian syntax: `> [!info]`, `> [!tip]`, `> [!quote]`
