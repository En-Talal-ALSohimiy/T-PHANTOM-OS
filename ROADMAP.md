# T‑PHANTOM OS Roadmap

This roadmap distinguishes **completed release work**, **active engineering work**, and **planned work**. Roadmap entries are not claims of current functionality unless they are explicitly marked as completed.

## Completed for the 5.3 public release line

- T‑PHANTOM OS user-facing identity and KDE Plasma integration.
- Arabic and English operating environment.
- VM validation for the current build.
- Physical-hardware / USB internal testing on tested hardware.
- AppArmor and nftables availability checks.
- Curated 44-entry cybersecurity tool-index validation.
- SHA‑256 publication for the exact released ISO.
- SourceForge primary public distribution.
- Google Drive secondary mirror.
- Public installation, integrity, security and release documentation.

## Near term

- Expand physical-device qualification across additional representative UEFI hardware.
- Build a documented compatibility matrix for Wi‑Fi, Ethernet, audio, graphics, storage and suspend/resume.
- Add genuine runtime screenshot coverage to the repository alongside presentation artwork.
- Improve first-run onboarding and bilingual operational documentation.
- Expand DFIR, incident-response, network-analysis and reverse-engineering workflow guides.
- Progressively integrate project-specific T‑PHANTOM cybersecurity tools after testing and stability validation.

## Security and reliability

- Repeatable pre-release system checks.
- Package and configuration regression tests.
- Installer validation across additional BIOS/UEFI scenarios.
- Stronger artifact provenance documentation.
- Review project-authored licensing separately from third-party package licensing.
- Formalize vulnerability handling and coordinated-disclosure workflow.
- Add signed release metadata when the release process supports it.

## Distribution engineering

- Maintain SourceForge as the primary public ISO distribution channel for the 5.3 line.
- Maintain an independent secondary mirror.
- Publish synchronized checksums and release notes across official channels.
- Automate release metadata generation.
- Build a dedicated T‑PHANTOM package/repository strategy for project-owned components.

## DFIR and security workflows

- Evidence-handling guidance.
- Incident-response playbooks.
- Network-analysis workflow references.
- Reverse-engineering workspace guidance.
- Controlled lab and training profiles.
- SOC-oriented workflow documentation where practical and testable.

## Long term

- Automated image-build pipeline.
- More reproducible release metadata.
- Hardware compatibility database.
- Hardened update and release channels.
- Dedicated repositories for T‑PHANTOM packages and project-authored tools.
- Community documentation and reviewed contributions.

> See the README and CHANGELOG for validated release capabilities. A planned item should not be presented as shipped until it passes the relevant validation.
