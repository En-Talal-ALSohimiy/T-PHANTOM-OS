<div align="center">

# T‑PHANTOM OS

### Cyber Forensics · DFIR · Authorized Penetration Testing · Reverse Engineering · Privacy

**نظام تشغيل أمني عربي/إنجليزي للتحقيق الجنائي الرقمي، الاستجابة للحوادث، الاختبار الأمني المصرح، التحليل العكسي والخصوصية.**

[![Release](https://img.shields.io/badge/release-5.3-35D8DC?style=for-the-badge)](#release)
[![Platform](https://img.shields.io/badge/platform-x86__64-0B1F26?style=for-the-badge)](#system-requirements)
[![Desktop](https://img.shields.io/badge/desktop-KDE%20Plasma-1D99F3?style=for-the-badge&logo=kde)](#desktop--identity)
[![Language](https://img.shields.io/badge/interface-Arabic%20%7C%20English-C9B56D?style=for-the-badge)](#bilingual-by-design)
[![SHA256](https://img.shields.io/badge/SHA--256-verified-success?style=for-the-badge)](#integrity)

**[English](#english) · [العربية](#العربية) · [Installation](docs/INSTALLATION.md) · [التثبيت بالعربية](docs/INSTALLATION_AR.md) · [Security](SECURITY.md) · [Roadmap](ROADMAP.md)**

</div>

---

## English

### What is T‑PHANTOM OS?

T‑PHANTOM OS is a security-focused Linux operating system built for practical cyber operations and digital investigation workflows. It provides a bilingual Arabic/English environment for **DFIR, digital forensics, authorized penetration testing, reverse engineering, incident response, security analysis, and privacy-oriented work**.

The project is designed around a clear principle: provide a focused, coherent workstation for security professionals instead of presenting an unstructured collection of tools.

### Core focus

| Area | Purpose |
|---|---|
| **DFIR** | Incident response, evidence handling, host and artifact analysis |
| **Digital Forensics** | Disk, file-system, registry, timeline and artifact investigation |
| **Authorized Pentesting** | Security assessment in systems where explicit authorization exists |
| **Reverse Engineering** | Binary and software analysis workflows |
| **Network Analysis** | Packet, protocol and DNS-oriented investigation |
| **Privacy** | A security-conscious workstation with reduced operational noise |
| **Bilingual UX** | Arabic and English localization for regional and international use |

### Designed for

- Digital forensics investigators
- DFIR and incident-response teams
- SOC and security analysts
- Authorized penetration testers
- Security researchers
- Reverse-engineering practitioners
- Cybersecurity students and training labs
- CTF and controlled lab environments

> **Authorization matters.** T‑PHANTOM OS is intended for lawful security work, education, research, and systems you own or are explicitly authorized to assess.

---

## العربية

### ما هو T‑PHANTOM OS؟

**T‑PHANTOM OS** نظام تشغيل أمني مخصص لبيئات الأمن السيبراني والتحقيق الجنائي الرقمي، ويقدم بيئة عملية ثنائية اللغة **العربية والإنجليزية** للعمل في مجالات:

- التحقيق الجنائي الرقمي **Digital Forensics**
- الاستجابة للحوادث **DFIR / Incident Response**
- الاختبار الأمني والاختراق المصرح **Authorized Penetration Testing**
- التحليل العكسي **Reverse Engineering**
- تحليل الشبكات والأدلة الرقمية
- الأبحاث الأمنية والخصوصية
- التدريب والمعامل الأكاديمية وبيئات CTF

الهدف ليس جمع أكبر عدد ممكن من الأدوات، بل بناء بيئة متماسكة وواضحة تساعد المختص على الوصول إلى أدواته ومسارات عمله بصورة منظمة.

### الفئات المستهدفة

المحققون الجنائيون الرقميون، فرق الاستجابة للحوادث، محللو SOC، مختبرو الاختراق المصرح لهم، الباحثون الأمنيون، الطلاب، الجامعات، مراكز التدريب، ومعامل الأمن السيبراني.

---

## Desktop & Identity

T‑PHANTOM OS includes a dedicated visual identity across the boot experience, installer, login screen, desktop, and system branding.

- Custom T‑PHANTOM boot identity
- T‑PHANTOM login experience
- KDE Plasma desktop
- Dark security-focused visual language
- Arabic and English environment
- Default hostname: `t-phantom`
- Dedicated **About Developer** desktop entry

---

## Bilingual by design

Arabic support is not treated as an afterthought. T‑PHANTOM is intended to work naturally for Arabic-speaking security practitioners while retaining correct English terminology for technical and international workflows.

---

## Release

| Item | Value |
|---|---|
| Product | **T‑PHANTOM OS** |
| Release line | **5.3** |
| Architecture | **x86_64 / amd64** |
| ISO filename | `T-PHANTOM.iso` |
| Desktop | KDE Plasma |
| Languages | Arabic + English |
| Boot media | USB / ISO / virtual machine |
| Status | Release candidate validated in VM; physical-device validation recommended before broad distribution |

### Integrity

Official ISO SHA‑256:

```text
86ed41941fcaaaafbf9042e9ea18f45b623c51a073cef461234ef7ff76f4d51a  T-PHANTOM.iso
```

Verify on Linux:

```bash
sha256sum T-PHANTOM.iso
```

The result must exactly match the published checksum above.

---

## Download

The ISO is approximately 4 GB and is **not stored directly in this GitHub repository**. Official download mirrors will be published here after final physical-device validation.

> Never trust an ISO distributed from an unofficial mirror unless its SHA‑256 matches the checksum published in this repository.

See [`SHA256SUMS`](SHA256SUMS).

---

## System requirements

Recommended baseline for installation or virtualization:

- 64-bit x86 processor
- 4 GB RAM minimum; 8 GB+ recommended for heavier analysis workflows
- 30 GB+ storage recommended
- UEFI-capable system recommended on modern hardware
- USB drive large enough for the ISO when creating installation media

Hardware support varies by chipset and device. Physical-hardware testing is part of release qualification.

---

## Installation

**English:** [`docs/INSTALLATION.md`](docs/INSTALLATION.md)  
**العربية:** [`docs/INSTALLATION_AR.md`](docs/INSTALLATION_AR.md)

> Installing T‑PHANTOM as the only operating system can erase all data on the selected disk. Confirm the target disk before writing partition changes.

---

## Project documentation

| Document | Purpose |
|---|---|
| [`docs/INSTALLATION.md`](docs/INSTALLATION.md) | Installation guide |
| [`docs/INSTALLATION_AR.md`](docs/INSTALLATION_AR.md) | دليل التثبيت بالعربية |
| [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md) | Project architecture and design principles |
| [`FAQ.md`](FAQ.md) | Frequently asked questions |
| [`ROADMAP.md`](ROADMAP.md) | Planned development |
| [`CHANGELOG.md`](CHANGELOG.md) | Release history |
| [`SECURITY.md`](SECURITY.md) | Vulnerability reporting |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Contribution guidelines |
| [`RELEASE_CHECKLIST.md`](RELEASE_CHECKLIST.md) | Release qualification checklist |
| [`NOTICE.md`](NOTICE.md) | Licensing and third-party notices |

---

## Current validated capabilities

The current release line has been tested for core OS identity, Arabic/English locale availability, AppArmor availability, nftables availability, the T‑PHANTOM desktop identity, installer flow, and a curated tool index.

Project qualification separates **tested** behavior from **planned** behavior. A feature is not described as validated until it has passed a reproducible test.

---

## Responsible use

T‑PHANTOM OS includes or may integrate security tools that can affect computers, networks, accounts, or data. Use them only in environments where you have explicit authorization.

The project does not endorse unauthorized access, disruption, credential theft, surveillance, or unlawful activity.

---

## Developer

**Design & Development:** Eng. Talal Fawaz Al‑Sohimiy  
**تصميم وتطوير:** م. طلال فواز السحيمي

- GitHub: [@En-Talal-ALSohimiy](https://github.com/En-Talal-ALSohimiy)
- Email: `en.talal.alsohimiy@gmail.com`
- Contact: `0544473041`
- Location: Saudi Arabia

---

<div align="center">

### T‑PHANTOM OS
**Security · DFIR · Authorized Pentest · Reverse Engineering · Privacy**

*Built with a security-first, evidence-driven release process.*

</div>
