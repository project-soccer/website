# Project Soccer — Website

Planned public website for [Project Soccer](https://github.com/project-soccer).

## Responsibility

Present the game, development status, and community entry points. The website may later link to or host the built browser client. It does not own authoritative gameplay, a separate account database, or an independent wallet backend.

## Boundaries

Game implementation belongs in `game/client`; application services belong in `game/server`, both in `project-soccer/game`. Do not duplicate their source or business rules here. Cross-project design belongs in `project-soccer/game` at `docs/game-design-and-architecture.md` (locally `../game/docs/game-design-and-architecture.md`).

## Status

Planning only. The public [project-soccer/website](https://github.com/project-soccer/website) repository was created with the founder’s authorization on 2026-09-20. Git operations use SSH. No website has been implemented or deployed. No framework, deployment provider, or license is selected for this repository.

All documentation must be written in English.

## Brand assets

The approved emblem with revised framing and transparency is available as a [GitHub avatar PNG](assets/brand/project-soccer-github-avatar-v1.png) with its [generation prompts and provenance](assets/brand/project-soccer-github-avatar-v1.md). The PNG is included in this repository; applying it as the GitHub organization avatar is a separate action. It does not establish the full brand identity.
