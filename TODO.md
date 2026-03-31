# TODO

--------------------------------------------------------------------------------
### - [x] 1--MARKDOWN--Added support for also parens as Markdown tasks:

- `( )` with background color red
- `(..)` with background color orange (WIP)
- `(x)` with background color green

**Approach:** Option D — Regex Mark plugin (Mara-Li/obsidian-regex-mark)
- Plugin config: regex `\( \)` → class `task-open` | regex `\(x\)` → class `task-done`
- CSS added to `theme.css` before the Style Settings block

--------------------------------------------------------------------------------
