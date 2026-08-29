# Security Policy

T‑PHANTOM OS is a security-focused operating system. Security reports are handled separately from normal feature requests and general support.

## Reporting a vulnerability

Please do **not** open a public GitHub issue for a vulnerability that could expose users, systems, credentials, or sensitive data.

Report security issues privately by email:

**talal@talalsuhaimi.com**

Include, when possible:

- affected T‑PHANTOM release or build
- affected component/package
- reproduction steps
- security impact
- logs or screenshots with sensitive data removed
- proof-of-concept details sufficient to reproduce safely
- suggested mitigation, if known

## Coordinated disclosure

Please allow reasonable time to reproduce, assess, fix, and validate an issue before public disclosure.

## Scope

Examples of security issues that should be reported privately include:

- privilege escalation
- insecure default permissions
- credential exposure
- unsafe update or package behavior
- boot-chain or installer security defects
- unintended remote exposure
- integrity-check bypasses
- vulnerabilities introduced by T‑PHANTOM-specific configuration or code

Upstream vulnerabilities in third-party software should normally also be reported to the relevant upstream project.

## Artifact integrity

The official T‑PHANTOM OS 5.3 ISO checksum is published in `SHA256SUMS` and `DOWNLOAD.md`. If a downloaded ISO does not match the published SHA‑256 exactly, do not boot or install it.

## Responsible use

Security tooling distributed with or documented by T‑PHANTOM is intended for lawful research, education, defensive operations, and explicitly authorized testing only.
