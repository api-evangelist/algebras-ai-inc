<!--
generated: 2026-07-17
method: searched
source: https://github.com/algebras-ai/algebras-skill/blob/main/skills/algebras/SKILL.md
note: Provider-published Agent Skill, saved verbatim below (original frontmatter preserved).
-->
---
name: algebras
description: Localize app translation files with Algebras CLI, including interactive config creation, glossary selection/download, multi-language translation, healthcheck review, and PO proofreader comments.
---

# Algebras Localization

Use this skill when the user asks to translate or localize files with Algebras, especially PO/gettext files and glossary-aware translation.

Follow the canonical workflow in `../../shared/algebras-localization-workflow.md`.

Prefer the helper scripts in `../../scripts/`:

- `algebras_configure.py` creates `.algebras.config` interactively.
- `algebras_glossaries.py` lists, selects, and downloads glossaries.
- `algebras_status.py` summarizes `algebras status` localized/not-localized/total key counts.
- `algebras_translate.py` translates one source file to one or more target languages.
- `algebras_healthcheck.py` summarizes `algebras healthcheck --format json` issues.
- `algebras_po_comments.py` adds `# used terms: original - translation` comments to PO files.

Never store `ALGEBRAS_API_KEY` in repo files. Ask the user to export it in their shell or CI secret store.
