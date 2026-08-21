# T‑PHANTOM OS FAQ

## Is T‑PHANTOM OS a general-purpose desktop distribution?

It can provide a normal Linux desktop, but its project focus is cybersecurity, DFIR, digital forensics, authorized penetration testing, reverse engineering, incident response, and privacy-oriented workflows.

## Is it intended for unauthorized hacking?

No. Security tools should only be used on systems you own or where you have explicit authorization.

## Does it support Arabic?

Yes. Arabic and English are part of the intended user experience and release validation.

## What desktop environment does it use?

KDE Plasma.

## What architecture is the current ISO built for?

x86_64 / amd64.

## What is the current ISO filename?

```text
T-PHANTOM.iso
```

## How do I verify the ISO?

Run:

```bash
sha256sum T-PHANTOM.iso
```

Expected SHA‑256:

```text
86ed41941fcaaaafbf9042e9ea18f45b623c51a073cef461234ef7ff76f4d51a
```

## Why is the ISO not hosted directly in this repository?

The current ISO is several gigabytes in size, so the repository is used for project documentation, checksums, issue tracking, release notes, and source/configuration material. Official download mirrors are linked separately.

## Can I install it as the only operating system?

Yes, but selecting the entire disk during installation can erase all existing data. Read the installation guide before proceeding.

## Is VM testing enough before production use?

No. VM validation proves important parts of the software path, but physical hardware introduces firmware, graphics, Wi‑Fi, audio, storage-controller, and power-management variables.

## Is T‑PHANTOM based on Linux?

Yes. It is a Linux operating system with a T‑PHANTOM-specific user-facing identity and security-focused configuration. Third-party and upstream component attribution remains preserved where required.

## Where should bugs be reported?

Normal bugs can be reported through GitHub Issues. Security vulnerabilities should be reported privately according to `SECURITY.md`.
