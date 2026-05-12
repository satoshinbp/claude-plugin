# Coding Conventions

## Naming

- **Use specific verbs** — Avoid vague verbs like `get`; choose words that describe the actual operation, such as `fetch` / `download` / `load`.
- **Avoid generic names** — Names like `tmp` / `retval` / `data` are prohibited in principle. `tmp` is allowed only for short-lived holding such as swapping two variables.
- **Include units in names** — For values with units, embed the unit in the variable name (e.g., `startMs`, `sizeMb`, `delaySec`).
- **Use `max` / `min` for bounds** — Do not use `limit`; make upper/lower bounds explicit, as in `maxItemsInCart` / `minAge`.
- **Use `first` / `last` for ranges** — Prefer `first` / `last` (inclusive on both ends) over `start` / `stop`.

## Comments

- **Do not state what the code already says** — Comments that merely repeat what function and variable names already convey are redundant; omit them.
- **Write the "why"** — Document intent, purpose, and background (why it is needed), not the step-by-step procedure.
- **Flag concerns and follow-ups** — Mark improvement ideas and concerns with `TODO` (handle later), `FIXME` (known defect), `HACK` (temporary workaround), or `XXX` (serious issue).
- **Summarize complex logic** — Prefix long or intricate blocks with a one-line statement of purpose.
- **Label each block's role** — When a function contains multiple distinct blocks, give each a one-line description of its role.
- **Avoid demonstratives** — Avoid vague references like "this" / "that"; name the subject concretely.
- **Describe the goal, not the mechanics** — For example, write "sort by descending price" rather than "reverse the list" — describe the desired outcome, not the operation.
