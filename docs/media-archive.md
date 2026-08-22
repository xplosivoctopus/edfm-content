# Media archive

Current public uploaded media binaries are stored as GitHub release assets instead of normal git files.

Latest package:

- Release: `media-current-2026-08-22`
- Asset: `edfm-media-current-20260822T035002Z.tar.zst`
- Size: `33,291,292` bytes
- SHA-256: `312321f0352200ce75e177bf355aa32c818410ad62d54cb147bb988382a3010e`
- File count: `33`

Download from the release page:

- `https://github.com/xplosivoctopus/edfm-content/releases/tag/media-current-2026-08-22`

## Package layout

After extraction, the package contains:

- `README.md`
- `manifest.json`
- `SHA256SUMS`
- `files/`

The `manifest.json` file lists each media file's source URL, description-page URL, MIME type, size, dimensions, source timestamp, MediaWiki SHA-1 metadata, archive path, and SHA-256 checksum.

## Relationship to file description pages

This repository's `pages/File/` directory contains the file description pages. Those pages are where licensing/source notes live. The release asset contains the corresponding binary files.

Use both together when restoring or rehosting media.

## Scope

The package contains current public upload binaries visible through MediaWiki's public file listing at build time.

It does not include:

- deleted files;
- suppressed/private files;
- database records;
- upload logs;
- user tables;
- historical versions of files.

## Verification

After downloading:

```bash
tar --zstd -xf edfm-media-current-20260822T035002Z.tar.zst
cd edfm-media-current-20260822T035002Z
sha256sum -c SHA256SUMS
```

Also verify the package itself:

```bash
sha256sum edfm-media-current-20260822T035002Z.tar.zst
```

Expected package SHA-256:

```text
312321f0352200ce75e177bf355aa32c818410ad62d54cb147bb988382a3010e
```
