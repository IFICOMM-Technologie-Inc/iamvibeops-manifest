# IAMVibeOps Manifest

[![License: CC BY-ND 4.0](https://img.shields.io/badge/license-CC%20BY--ND%204.0-lightgrey)](LICENSE)
[![Latest release](https://img.shields.io/github/v/release/IFICOMM-Technologie-Inc/iamvibeops-manifest?label=manifest)](https://github.com/IFICOMM-Technologie-Inc/iamvibeops-manifest/releases/latest)

**Intelligence Artificial Manifest for Operational Execution**

An independent authorial work by **Agenor Mota** — Lévis, Québec, Canada — 2026.

> Human intention begins. Diagnosis guides. Backlog organizes. Agents execute. Evidence proves. Governance preserves trust.
>
> **IAMVibeOps — I AM. Human intention. AI execution. Evidence-based operations.**

---

## Download the manifesto

The official PDFs are published as **release assets**, in four languages:

➡️ **[Get the latest release](https://github.com/IFICOMM-Technologie-Inc/iamvibeops-manifest/releases/latest)**

| Language | File |
|---|---|
| English (canonical) | `IAMVibeOps-Manifest-v1.0-EN.pdf` |
| Français | `IAMVibeOps-Manifest-v1.0-FR.pdf` |
| Português | `IAMVibeOps-Manifest-v1.0-PT.pdf` |
| Español | `IAMVibeOps-Manifest-v1.0-ES.pdf` |

Each release also includes `SHA256SUMS-release.txt` and OpenTimestamps proofs (`*.ots`).

## Verify integrity (SHA-256)

Download a PDF plus `SHA256SUMS-release.txt` into the same folder, then:

```bash
# macOS
shasum -a 256 -c SHA256SUMS-release.txt
# Linux
sha256sum -c SHA256SUMS-release.txt
```

`OK` next to each file means it has not been altered.

## Verify authorship date (OpenTimestamps)

Each artifact ships with an OpenTimestamps proof (`<file>.ots`) anchoring its date
of existence to the Bitcoin blockchain — independently verifiable, with no trust in
GitHub or the author required.

```bash
pipx install opentimestamps-client            # once

# Verify a PDF against its proof (both files in the same folder):
ots verify IAMVibeOps-Manifest-v1.0-EN.pdf.ots

# If it reports the proof is still "pending", complete it first:
ots upgrade IAMVibeOps-Manifest-v1.0-EN.pdf.ots
```

A successful verification prints the Bitcoin block timestamp at which the file
provably already existed.

## License

The manifesto **content** (text and PDFs) is licensed under
**[Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)](LICENSE)**.

You are free to **share and redistribute the manifesto, in whole and unaltered,
including commercially**, provided you give attribution to
*"Agenor Mota — IAMVibeOps Manifest"* and link back to this repository.
You may **not** distribute modified, abridged or remixed versions.

The **"IAMVibeOps" name and marks** and the **confidential method** behind the
framework are **not** licensed and remain reserved. See [COPYRIGHT.md](COPYRIGHT.md).

© 2026 Agenor Mota / IFICOMM Technologie Inc.

## Links

- Website: [iamvibeops.com](https://iamvibeops.com)
- Releases: [github.com/IFICOMM-Technologie-Inc/iamvibeops-manifest/releases](https://github.com/IFICOMM-Technologie-Inc/iamvibeops-manifest/releases)
