# T‑PHANTOM OS Architecture

T‑PHANTOM OS is organized as a security-focused Linux workstation with a deliberately separated release process: **upstream base, identity, desktop, installer, security controls, curated tools, project-specific components, documentation, validation, and release publication** are treated as distinct layers.

## Upstream foundation

T‑PHANTOM OS is developed on top of Linux and uses upstream components from the Debian/Kali and KDE ecosystems. Upstream licenses, copyrights, trademarks and attribution requirements remain applicable to their respective components. T‑PHANTOM-specific engineering does not imply authorship over upstream projects.

## Design principles

### 1. Evidence-driven releases

A feature is described as validated only after a reproducible test. Planned or private development work remains explicitly separated from public release claims.

### 2. Security-first defaults

The project favors understandable, auditable security controls over opaque customization. Current 5.3 validation includes AppArmor and nftables availability.

### 3. Curated tools, not tool-count marketing

T‑PHANTOM aims to organize useful workflows for DFIR, forensics, incident response, authorized testing, network analysis, reverse engineering and security research rather than maximizing the number of installed tools.

The current 5.3 internal audit reviewed **44 indexed cybersecurity tool entries**. That number describes the tested index for the current release line, not a claim of external certification or superiority over other distributions.

### 4. Bilingual operation

Arabic and English are treated as first-class user environments. Technical terminology remains accurate in English while Arabic documentation and UI support regional practitioners.

### 5. Independent user-facing identity

The product presents itself to users as **T‑PHANTOM OS** across major operating-system touchpoints while preserving required upstream attribution and licensing.

### 6. Progressive project-owned tooling

Project-specific cybersecurity tools designed and programmed for T‑PHANTOM are introduced progressively after testing and stability validation. Private/development tools are not considered part of the public release unless explicitly documented as shipped.

## Major layers

### Boot and installation

- boot menu
- live environment
- installer
- disk installation
- bootloader

### Desktop

- KDE Plasma
- T‑PHANTOM wallpaper and look-and-feel
- T‑PHANTOM login identity
- Arabic/English locales
- developer information entry

### Security controls

- AppArmor
- nftables
- Linux permissions and privilege separation
- release integrity checks

### Security tool layer

Tools are indexed and grouped around practical workflows. The exact package set may evolve between releases; release documentation should reflect what was actually validated.

### Project-specific component layer

This layer can contain T‑PHANTOM-authored configuration, automation, scripts, utilities and cybersecurity tools. Authorship claims must remain limited to components actually created by the project.

### Release engineering

The release process includes:

1. source/configuration changes
2. package/tool validation
3. image build
4. boot testing
5. installer testing
6. installed-system testing
7. visual identity review
8. checksum generation
9. physical-hardware / USB qualification on tested hardware
10. mirror publication
11. release-documentation synchronization

## Distribution model

For the T‑PHANTOM OS 5.3 public release line:

- **Primary binary distribution:** SourceForge
- **Secondary mirror:** Google Drive
- **Project development/documentation:** GitHub
- **Integrity reference:** published SHA‑256 in this repository and the release files

## Trust model

Users should verify ISO artifacts against the SHA‑256 published in this repository. Official mirrors should be treated as transport; the checksum is the integrity reference for the released image.

Current 5.3 SHA‑256:

```text
86ed41941fcaaaafbf9042e9ea18f45b623c51a073cef461234ef7ff76f4d51a  T-PHANTOM.iso
```

Future releases may expand the trust model with signed metadata, dedicated project package repositories, stronger provenance controls and a more automated build/release pipeline.
