# AUTHORSHIP & INTEGRITY RECORD

## Authorship

| Field | Value |
|---|---|
| Work | IAMVibeOps Manifest — Intelligence Artificial Manifest for Operational Execution |
| Author | Agenor Mota |
| Location | Lévis, Québec, Canada |
| Year | 2026 |
| Version | 1.0 — Public Introduction |
| Status | PUBLIC VERSION 1.0 |
| Primary domain | iamvibeops.com |
| Copyright | © 2026 Agenor Mota. All rights reserved. |

## Publication model: private source + public PDFs

This source repository may be kept **private**. The **public** record of authorship
is published separately as:

1. the **PDF exports** (in a separate public repository and/or on iamvibeops.com), and
2. their **OpenTimestamps proofs** (`.ots`), which give a public, independent date
   of existence that does **not** depend on this repository being public.

This keeps full control of the source while still producing strong public evidence.

## How authorship validity is established

1. **OpenTimestamps proofs (`.ots`)** — the release workflow timestamps the PDFs
   and the `SHA256SUMS-release.txt` against public calendar servers, anchored to
   the Bitcoin blockchain. Anyone can verify the date of existence with
   `ots verify <file>.ots` against the original file — no access to this repo
   required. This is the primary public anchor when the source repo is private.
2. **Content integrity hashes** — SHA-256 of each canonical source file is
   recorded in `checksums/SHA256SUMS.txt` (and per-release in
   `SHA256SUMS-release.txt`), so anyone can verify the files were not altered.
3. **Immutable commit history + signed tags** — even in a private repo, signed
   commits (`git commit -S`) and signed tags (`git tag -s`) bind the author to
   the content and date; if later made public, they corroborate the record.

### Verifying an OpenTimestamps proof

```bash
pipx install opentimestamps-client          # once
ots upgrade SHA256SUMS-release.txt.ots       # complete the Bitcoin attestation (after a few hours)
ots verify  SHA256SUMS-release.txt.ots       # verify against the original file in the same folder
```

> Note: timestamping + hashing provide strong *evidence* of priority of date, but
> are **not a substitute for formal protections** (copyright registration,
> trademark filing). See "Pending formal steps" below.

## PDF integrity hashes (pending)

The canonical documents declare that the **PDF SHA-256** is "to be generated after
final PDF export." Record them here once the PDFs are produced:

| Language | PDF file | SHA-256 |
|---|---|---|
| EN | IAMVibeOps-Manifest-v1.0-EN.pdf | _pending_ |
| FR | IAMVibeOps-Manifest-v1.0-FR.pdf | _pending_ |
| PT | IAMVibeOps-Manifest-v1.0-PT.pdf | _pending_ |
| ES | IAMVibeOps-Manifest-v1.0-ES.pdf | _pending_ |

Generate with:

```bash
shasum -a 256 IAMVibeOps-Manifest-v1.0-EN.pdf
```

## Pending formal steps (outside this repository)

- [ ] Final PDF export of each language version + record SHA-256 above.
- [ ] Formal legal review of disclaimer and independence wording.
- [ ] Trademark search for "IAMVibeOps" (CIPO — Canada) before any TM claim.
- [ ] Optional copyright registration.
- [ ] Optional patentability assessment (do not assert patentability publicly).
