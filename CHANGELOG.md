# Changelog

All notable T‑PHANTOM OS release changes are documented here.

## 5.3 — 2026-08-21

### Added

- T‑PHANTOM user-facing operating-system identity.
- Arabic and English locale support.
- KDE Plasma desktop integration.
- T‑PHANTOM wallpaper and visual identity.
- Branded boot, installer, login and desktop experience.
- Default hostname target: `t-phantom`.
- About Developer desktop entry and local information page.
- Curated indexed security-tool set.
- AppArmor validation.
- nftables validation.
- Installation and release documentation.

### Validated

- boot menu and installer flow
- installed-system boot
- OS identity
- Arabic/English locale configuration
- AppArmor availability
- nftables availability
- desktop wallpaper and login identity
- developer shortcut
- curated security-tool index
- VM execution on the current build
- physical-hardware / USB internal testing on tested hardware

The internal 5.3 tool-index audit covered **44 indexed cybersecurity entries** and completed without a tool-index miss/warn in that validation run.

### Hardware scope

Physical-hardware validation describes the machines actually tested; it is not a universal compatibility certification. Wi‑Fi, graphics, audio, storage controllers, firmware and power-management behavior can vary by device.

### ISO

```text
T-PHANTOM.iso
```

SHA‑256:

```text
86ed41941fcaaaafbf9042e9ea18f45b623c51a073cef461234ef7ff76f4d51a
```

## 5.3 distribution update — 2026-08-29

- Published the 5.3 ISO to SourceForge as the primary public download.
- Kept Google Drive as a secondary mirror.
- Published `README.txt` and `SHA256SUMS.txt` alongside the SourceForge ISO.
- Verified that the SourceForge 4.1 GB ISO download starts successfully.
- Aligned GitHub download documentation with the SourceForge release.
- Updated the official security contact to `talal@talalsuhaimi.com`.
- Added dedicated 5.3 release notes.

Primary download:

https://sourceforge.net/projects/t-phantom-os/files/T-PHANTOM-OS-5.3/T-PHANTOM.iso/download
