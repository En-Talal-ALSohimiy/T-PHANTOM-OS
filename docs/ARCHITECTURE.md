# T‑PHANTOM OS Architecture

T‑PHANTOM OS is organized as a security-focused Linux workstation with a deliberately separated release process: **identity, desktop, installer, security controls, curated tools, documentation, and release verification** are treated as distinct layers.

## Design principles

### 1. Evidence-driven releases

A feature is described as validated only after a reproducible test. Planned work remains explicitly labeled as planned.

### 2. Security-first defaults

The project favors understandable, auditable security controls over opaque customization. Current release validation includes AppArmor and nftables availability.

### 3. Curated tools, not tool-count marketing

T‑PHANTOM aims to organize useful workflows for DFIR, forensics, incident response, authorized testing, network analysis, and reverse engineering rather than maximizing the number of installed tools.

### 4. Bilingual operation

Arabic and English are treated as first-class user environments. Technical terminology remains accurate in English while Arabic documentation and UI support regional practitioners.

### 5. Independent user-facing identity

The product presents itself to users as **T‑PHANTOM OS** across the major operating-system touchpoints while preserving required upstream attribution and licensing internally.

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
9. physical-hardware qualification
10. publication

## Trust model

Users should verify ISO artifacts against the SHA‑256 published in this repository. Official mirrors should be treated as transport; the checksum is the integrity reference for the released image.

Future releases may expand the trust model with signed metadata and a more automated build/release pipeline.
