# Project Soccer — Website

Planned public website for [Project Soccer](https://github.com/project-soccer).

## Responsibility

Present the game, development status, and community entry points. The website may later link to or host the built browser client. It does not own authoritative gameplay, a separate account database, or an independent wallet backend.

## Boundaries

Game implementation belongs in `game/client`; application services belong in `game/server`, both in `project-soccer/game`. Do not duplicate their source or business rules here. Cross-project decisions are in `project-soccer/game` under `docs/adr/`; current behavior belongs in `docs/specifications/`.

## Status

Planning only. The public [project-soccer/website](https://github.com/project-soccer/website) repository was created with the founder’s authorization on 2026-09-20. Git operations use SSH. No website has been implemented or deployed. No framework, deployment provider, or license is selected for this repository.

All documentation must be written in English.

## Brand assets

<img src="assets/brand/project-soccer-logo.svg" width="160" alt="Project Soccer football and PS monogram">

Use the [SVG master](assets/brand/project-soccer-logo.svg) for scalable graphics and the [PNG export](assets/brand/project-soccer-logo.png) for raster uploads. The football interior is opaque; only the exterior is transparent. See [provenance and format notes](assets/brand/project-soccer-logo.md). The older generated avatar remains in Git history. Applying the organization avatar is a separate action.
