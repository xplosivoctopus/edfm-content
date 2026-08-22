# Importing the current-content archive

This repository is a current-page archive, not a full MediaWiki database backup. It is designed to preserve readable/reusable public EDFM content if the live site is unavailable.

## Archive layout

- `manifest.json` lists every exported page, source URL, namespace, page ID, revision ID, timestamp, and file path.
- `pages/Main/` contains article-space pages.
- `pages/Template/` contains templates.
- `pages/Module/` contains Scribunto/Lua modules.
- `pages/Category/` contains category pages.
- `pages/Project/` contains EDFM project/policy pages.
- `pages/MediaWiki/` contains public interface-message pages.
- `pages/File/` contains file description pages, not binary media files.

Each `.wiki` file begins with an HTML comment containing source metadata, followed by current wikitext.

## Basic recovery options

### Option A: read directly from GitHub

For emergency access, articles can be read as plain wikitext directly from this repository.

### Option B: import into MediaWiki

A future maintainer can import pages into a fresh MediaWiki install by using a script that:

1. reads `manifest.json`;
2. orders imports roughly by namespace, importing templates/modules before article pages;
3. strips or keeps the metadata comment according to the new site's preference;
4. writes each page using a maintenance/API account;
5. reviews templates/modules/interface pages for compatibility with the new MediaWiki version.

Recommended import order:

1. `Module`
2. `Template`
3. `MediaWiki`
4. `Category`
5. `Project`
6. `File`
7. `Main`

### Option C: build a static mirror

A static mirror can be generated from the wikitext or from live rendered HTML snapshots in a future export. This repository currently stores source wikitext only.

## What this archive cannot restore by itself

This archive does not include:

- account data;
- page revision history;
- deleted or suppressed pages;
- logs;
- uploaded binary files;
- site configuration;
- extensions;
- database tables.

For a full restoration of the original site, a trusted operator needs a separate encrypted disaster-recovery backup.

## Licensing and attribution

Reuse should preserve EDFM licensing and attribution requirements, including any source/license notes on individual file description pages and project policy pages.
