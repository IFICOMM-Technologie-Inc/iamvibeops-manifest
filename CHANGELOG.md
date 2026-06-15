# Changelog

All notable changes to the IAMVibeOps Manifest public repository.

## [1.0] — 2026-06-14

### Added
- IAMVibeOps Manifest v1.0 — Public Introduction, in EN (canonical), FR, PT, ES.
- Public Introduction Notice, Independence Statement and Non-disclosed Materials sections.
- Legal Disclaimer ("as is") clause in all four language versions.
- Authorship & integrity record (`AUTHORSHIP.md`), copyright/use notice (`LICENSE`), and `NOTICE.md`.
- Source-file SHA-256 checksums (`checksums/SHA256SUMS.txt`).

### Licensing
- Manifesto content (text + PDFs) licensed under **CC BY-ND 4.0** (`LICENSE`, verbatim legal code); reservations of name/marks and confidential method recorded in `COPYRIGHT.md`. Included code is MIT.

### Integrity & automation
- `verify.sh` + CI (`.github/workflows/verify.yml`) check source SHA-256 on every push/PR.
- Release workflow (`.github/workflows/release.yml`) renders PDFs, computes SHA-256, and **timestamps artifacts with OpenTimestamps** (`.ots`) attached to the Release.
- Publication model: source repo may be **private**; PDFs + `.ots` proofs are published publicly (separate repo / iamvibeops.com), giving public proof of date without exposing the source.

### Notes
- Source markdown derived faithfully from the authored `.docx` originals.
- PT §2 wording aligned with EN/FR/ES ("questão essencial" / essential question) — editorial consistency only; no change of meaning.
- PDF SHA-256 per language remains pending until final PDF export.
