# Elite Dangerous Field Manual — current content archive

This repository contains a current-only public content export from [Elite Dangerous Field Manual](https://edfieldmanual.com/).

It is intended as a continuity archive so the public wiki content can survive if the live site becomes unavailable.

## What is included

- Current wikitext for public content namespaces.
- Page metadata needed to trace each exported page back to its current live revision.
- `manifest.json` listing exported pages and source revision IDs.

## What is not included

This archive intentionally does **not** include:

- the MediaWiki database;
- revision history;
- user accounts, emails, password hashes, sessions, tokens, or OAuth data;
- logs, deleted pages, suppressed/private revisions, abuse logs, or checkuser data;
- server configuration, DNS/Cloudflare details, secrets, or backups;
- uploaded binary media files in this first export.

## Export details

- Exported at UTC: `2026-08-22T03:36:48Z`
- Page count: `633`
- Format: current MediaWiki wikitext, one page per `.wiki` file

## Continuity and import docs

- `docs/continuity.md` explains the purpose and emergency handoff model for this archive.
- `docs/importing-current-content.md` explains how a future maintainer can reuse or import the exported wikitext.
- `docs/media-archive.md` explains the current uploaded-media release package.

## Restore/reuse notes

These files are not a full MediaWiki backup. They are a public content archive. A future maintainer can import or adapt the wikitext into a new wiki, static site, or documentation system, subject to EDFM's licensing and attribution requirements.
