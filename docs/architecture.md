# Repository and architecture plan

## Repository arrangement

Use this repository, `octocl/event-card-planning`, for planning documents under `docs/`. The separate public repositories `octocl/event-card-backend` and `octocl/event-card-frontend` are linked here at `backend/` and `frontend/` as Git submodules. Their initial files are placeholders; no implementation has started. Add a mobile app or another service repository only when needed. See [submodules.md](submodules.md) for the workflow.

## Design principles (proposed, not a chosen stack)

- Store event and invitation content separately from template presentation, so switching designs preserves entered details.
- Give each hosted invitation a stable identifier and link; paid owner edits should update the webpage at that link. Decide autosave and publish timing later.
- Design webpage and image rendering as reusable outputs from shared invitation data. Downloaded images remain static and require regeneration after edits. Decide how much layout the outputs share after exploring examples.
- Structure localized UI strings and invitation content to support later language expansion, including different scripts and text directions.
- Keep optional guest, RSVP, and media capabilities modular if they are added later. Leave payment package and output entitlement rules configurable until pricing is decided.

No frontend or backend framework, hosting provider, database, sign-in method, rendering approach, or deployment plan has been selected. Those choices follow the product decisions in [decisions.md](decisions.md).
