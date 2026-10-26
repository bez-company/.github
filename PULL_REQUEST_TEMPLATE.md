<!--
Short on purpose: a person should understand the change from the title and this body in under a minute.
Title and body in English, Conventional Commits in the title: `[BEZ-<n>] type(scope): effect for the user`.
Delete this comment and every line that does not apply.

SCREEN CHANGE: ONE image, before and after side by side:  pr-visual compare before.png after.png
  New screen (no "before"): one sheet:  pr-visual sheet a.png b.png ...
  Desktop and mobile each get their own image. Light and dark when the theme changes. Fake data only.
  Upload:  scripts/pr-assets.sh <folder> <png>... (or pr-visual upload) and paste the markdown it prints, untouched: the ?raw=true matters.

LOGIC, DATA OR FLOW CHANGE: draw the flow right here in Mermaid (GitHub renders it), never as an image. Small, up to ~10 nodes:
  input, what happens, output, what happens on failure.
  sequenceDiagram: steps between systems or people | flowchart TD: decision rules | stateDiagram-v2: states of a record
  erDiagram: touched tables only | routes: table Route, Permission, Request, Responses | config: table Variable, Where it is set, Default
  No diagram clarifies? A Before | After table is enough.
-->
ClickUp: [card name](https://app.clickup.com/t/<id>)

<One or two sentences: what changes, for whom, and why. Link the SPEC or ADR if there is one.>

![](<screen change: ONE image, before | after>)

```mermaid
<logic, data or flow change: the diagram, here>
```

**Verified:** <what was actually exercised: tests, a real browser, a real database>
**Not verified:** <what was not, said plainly>
**Rollback:** <revert, flag, or "migration is additive">; delete if trivial
