# Hookshot / Longshot status tracker

This is a **no-game-files** editorial status tracker for unofficial PC projects related to *The Legend of Zelda: Ocarina of Time* (especially the Switch 2 remake trees and related tools).

The full comparison, source directory and install notes live on **[hookshotgithub.com](https://hookshotgithub.com/)**:

- [Status and timeline](https://hookshotgithub.com/status/)
- [Sources and mirrors](https://hookshotgithub.com/mirrors/)
- [Install notes](https://hookshotgithub.com/install/)
- [Ocarina of Time on PC](https://hookshotgithub.com/ocarina-of-time-pc/)
- [Longshot notes](https://hookshotgithub.com/longshot/)

This repository does **not** replace those pages. It exists so the same point-in-time checks can be read as markdown and as `status.json`.

The snapshot in this commit was assembled on **2026-11-24**, after a fresh official-source recheck. Availability and tags can change after `last_checked`.

## Red line

**Do not open issues or pull requests that add, request, or link to game files.**

This tracker does not host, mirror, or link to:

- ROMs, dumps, `.nup` / `.nsp` / `.xci` packages, or packed game builds
- ready-made game executables
- keys, firmware, or other console secrets

Links below go to project websites, source repositories, or documentation only. Owning a game does not by itself settle every legal question; follow each project’s own requirements and the law where you are.

This is an independent tracker, not Nintendo, GitHub, NotRexed, Team MagicBean, or any of the other listed maintainers.

## How to read the timeline

[`TIMELINE.md`](TIMELINE.md) is a short, sourced chronology derived from the live [status page](https://hookshotgithub.com/status/) plus later editorial rechecks that could be verified from public sources. A date is a reported or checked date, not a legal conclusion. A 404 confirms that an address was unavailable at the time of the check; it does not by itself prove a DMCA takedown or any other cause.

## How to read `status.json`

[`status.json`](status.json) is a stable, machine-readable snapshot.

- `schema` — current schema id: `hookshotgithub-status-v1`
- `timezone` — timestamps are intended to be read in `Asia/Shanghai` (UTC+8) and are labeled as such
- `last_checked` — when this snapshot was assembled
- `site` — canonical comparison site
- `projects[]` — one object per tracked entry:
  - `id` — stable slug
  - `name` — display name
  - `type` — `static_recompilation`, `emulator`, `original_port`, `utility`, `mirror`, or `endpoint`
  - `maintainer` — person, team, or host as publicly identified
  - `url` — project or documentation landing page (not a game download)
  - `version_or_status` — latest listed tag, HTTP result, or short status string
  - `last_checked` — when *that* entry was last verified, labeled with timezone
  - `notes` (optional) — short editorial caveat

Nightlies and other pre-releases are recorded when they are the item actually listed, but they are not treated as a stable-version guarantee. These checks are not an uptime monitor, a safety certification, or an endorsement.
