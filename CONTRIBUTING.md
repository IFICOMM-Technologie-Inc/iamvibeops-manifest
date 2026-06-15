# Contributing

Thank you for your interest in the **IAMVibeOps Manifest**.

This repository is **not a conventional open-source project**. It is the public
source of record for an **authored work** by Agenor Mota, published to establish a
clear, timestamped record of authorship. Please read this before opening an issue
or pull request.

## What this means

- The **manifesto text is fixed and authorial.** Pull requests that rewrite,
  reinterpret, expand or alter the meaning of the manifesto body
  (`manifest/*.md`) will **not** be accepted. The wording is part of the authored
  work and its versioned record.
- Authorship, copyright and reuse terms are defined in [LICENSE](LICENSE) and
  [NOTICE.md](NOTICE.md). All rights are reserved.

## What is welcome

You may open an **issue** for:

- **Typos or grammar** in any language version (EN / FR / PT / ES).
- **Translation fidelity** concerns — a passage that diverges in meaning from the
  canonical English version.
- **Broken links, formatting or rendering** problems.
- **Integrity questions** — if `./verify.sh` fails or a checksum looks wrong.

For typo/translation fixes, a small, surgical pull request is acceptable **only if
it does not change meaning**. Substantive wording belongs to the author and is
handled as a new manifesto version.

## Integrity rules for any accepted change

- If a file under `manifest/` changes, the checksums must be regenerated:
  `./verify.sh --update`, and the change recorded in [CHANGELOG.md](CHANGELOG.md).
- Never add confidential or operational material to this **public** repository
  (prompts, playbooks, diagnostic models, scoring, templates, consulting
  materials, secrets). See [NOTICE.md](NOTICE.md).

## Versioning

Material changes produce a **new version** (e.g. `v1.1`), a new changelog entry,
and a new signed tag — they do not silently overwrite `v1.0`.

## Contact

Via [iamvibeops.com](https://iamvibeops.com).
