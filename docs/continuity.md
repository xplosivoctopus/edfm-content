# Continuity purpose

This repository exists so the public EDFM knowledge base can survive if the live site becomes unavailable.

It is intended for:

- emergency public access to current article/source text;
- future rehosting or migration work;
- preservation of templates, modules, categories, project pages, and public file description pages;
- periodic snapshots of current public content.

It is not intended to be a full operational backup.

## Relationship to the source repository

The source/config-example repository is:

- `https://github.com/xplosivoctopus/edfm`

This content archive pairs with that repository:

- `edfm` preserves EDFM-specific code, assets, examples, and tests.
- `edfm-content` preserves current public wiki content.

Together they are enough to help someone rebuild a readable EDFM-derived site. They are not enough to restore the original server exactly.

## Update cadence

This archive is designed to be refreshed from the live wiki on a recurring schedule. Each refresh exports current public page text only.

## Emergency handoff checklist

If the live site is unavailable and the maintainer cannot be reached:

1. Clone this repository.
2. Review `README.md` and `docs/importing-current-content.md`.
3. Clone `https://github.com/xplosivoctopus/edfm` for source/config examples.
4. Decide whether the immediate goal is a static mirror or a new MediaWiki install.
5. Preserve attribution and licensing information.
6. If a trusted encrypted disaster-recovery package is available, use that for full restoration instead of this content-only archive.

## Boundaries

Do not add private operational material to this repository. In particular, keep out:

- raw database dumps;
- user/account data;
- logs;
- credentials;
- live configuration files;
- deleted/private/suppressed content;
- unreviewed binary uploads.
