# CLAUDE.md — Things Theme for Obsidian

## Project Overview

**Things** is a community CSS theme for [Obsidian](https://obsidian.md), inspired by the design of the [Things 3](https://culturedcode.com/things/) task manager app. It provides a clean, native-feeling UI for macOS and iOS users, with support for light/dark modes, custom checkboxes, and several community plugins.

- **Author:** @colineckert
- **Current version:** 2.1.20 (see `manifest.json`)
- **Min Obsidian version:** 1.0.0
- **Main file:** `theme.css` (primary stylesheet — this is where all work happens)

## Repository Structure

```
theme.css        — Main theme stylesheet (all styling lives here)
obsidian.css     — Legacy/compatibility stylesheet
manifest.json    — Theme metadata (name, version, author)
README.md        — Public documentation for users
assets/          — Screenshots and images for README
.github/         — GitHub funding configuration
```

## Development Guidelines

- All changes to the theme go in `theme.css`.
- CSS variables are defined at the top of `theme.css` under `body {}`.
- Color palette uses named variables: `--blue`, `--pink`, `--green`, `--yellow`, `--orange`, `--red`, `--purple`.
- Heading colors, strong/em colors, and quote colors are controlled via CSS variables.
- Style Settings plugin compatibility: customizable properties must follow the Style Settings annotation format in CSS comments.
- Keep section comments using the `/* ─── Section Name ─── */` style already used throughout the file.
- Bump the version in both `manifest.json` and the comment header in `theme.css` when releasing.

## Supported Plugins

Changes affecting plugin-specific styles should be tested against:
- Kanban (`obsidian-kanban`)
- Calendar (`obsidian-calendar-plugin`)
- Style Settings (`obsidian-style-settings`)
- Checklist (`obsidian-checklist-plugin`)
- Hider (`obsidian-hider`)

## Git Commits

- Do **not** include `Co-Authored-By` lines in commit messages.

## Language Policy

> **IMPORTANT:** The user may communicate in Spanish, but Claude Code must always respond in English.
> All programming, documentation, comments, and responses must be in English.
> Only respond or create files in Spanish if the user explicitly requests it.

### Default English Markdown Files

The following files must always be written in English by default:

- `CLAUDE.md`
- `TODO.md`
- `IDEAS.md`
- `README.md`
