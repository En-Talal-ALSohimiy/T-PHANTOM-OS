# Contributing to T‑PHANTOM OS

Thank you for helping improve T‑PHANTOM OS.

## Before contributing

- Keep security, reliability, and reproducibility ahead of feature count.
- Preserve accurate technical attribution and third-party licensing.
- Do not describe planned work as implemented or validated.
- Keep Arabic and English documentation aligned when changing user-facing behavior.
- Do not submit content that facilitates unlawful access or abuse.

## Good contribution areas

- documentation corrections
- Arabic/English localization improvements
- hardware compatibility reports
- installer and boot regression reports
- DFIR workflow documentation
- packaging fixes
- usability improvements
- security-hardening proposals
- automated tests and release checks

## Bug reports

A useful report includes:

1. T‑PHANTOM release/build.
2. Hardware or VM configuration.
3. Exact steps to reproduce.
4. Expected result.
5. Actual result.
6. Relevant logs/screenshots with secrets removed.
7. Whether the issue reproduces consistently.

## Security reports

Do not open a public issue for an exploitable security defect. Follow `SECURITY.md`.

## Pull requests

Keep pull requests focused. Explain what changed, why it changed, how it was tested, and whether the change affects boot, installer, security configuration, localization, or release artifacts.

## Validation standard

A change is not considered complete merely because it builds. Depending on scope, validation may include:

- syntax/static checks
- boot testing
- live-session testing
- clean installation testing
- post-install reboot testing
- hardware testing
- checksum verification
- bilingual UI review

The goal is evidence-driven releases rather than assumptions.
