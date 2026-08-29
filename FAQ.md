# T‑PHANTOM OS FAQ

## Is T‑PHANTOM OS a general-purpose desktop distribution?

It can provide a normal Linux desktop, but its project focus is cybersecurity, DFIR, digital forensics, authorized penetration testing, reverse engineering, incident response, network analysis, security research, and privacy-oriented workflows.

## Is it intended for unauthorized hacking?

No. Security tools should only be used on systems you own or where you have explicit authorization.

## Does it support Arabic?

Yes. Arabic and English are part of the intended user experience and release validation.

## What desktop environment does it use?

KDE Plasma.

## What architecture is the current ISO built for?

x86_64 / amd64.

## What is the current release?

T‑PHANTOM OS 5.3.

## What is the current ISO filename?

```text
T-PHANTOM.iso
```

## Where is the official download?

The primary public download is SourceForge:

https://sourceforge.net/projects/t-phantom-os/files/T-PHANTOM-OS-5.3/T-PHANTOM.iso/download

Google Drive is maintained as a secondary mirror:

https://drive.google.com/file/d/1naFZI6lveSYTdfP-UqyewSRyHx8tuEIF/view?usp=sharing

## How do I verify the ISO?

Run on Linux:

```bash
sha256sum T-PHANTOM.iso
```

Or on Windows PowerShell:

```powershell
Get-FileHash .\T-PHANTOM.iso -Algorithm SHA256
```

Expected SHA‑256:

```text
86ed41941fcaaaafbf9042e9ea18f45b623c51a073cef461234ef7ff76f4d51a
```

## Why is the ISO not hosted directly in this GitHub repository?

The ISO is approximately 4.1 GB. GitHub is used for project documentation, checksums, issue tracking, release notes, source/configuration material, and project development. SourceForge is the primary public binary-distribution host.

## Can I install it as the only operating system?

Yes, but selecting the entire disk during installation can erase all existing data. Read the installation guide before proceeding.

## Has T‑PHANTOM been tested on physical hardware?

Yes. The current 5.3 build has undergone internal physical-hardware / USB testing on tested hardware. That does not mean every computer is guaranteed compatible; firmware, Wi‑Fi, graphics, audio, storage and power-management behavior vary by device.

## What does the 44-tool validation mean?

The current internal audit reviewed 44 indexed cybersecurity tool entries and completed without a tool-index miss/warn in that validation run. It is a validation of the indexed set, not an external certification of every upstream tool or every possible workflow.

## Does T‑PHANTOM contain original project tools?

Project-specific cybersecurity tools designed and programmed for T‑PHANTOM are being introduced progressively after testing and stability validation. Private or development tools should not be assumed to be part of the public 5.3 ISO unless the release documentation explicitly says so.

## Is T‑PHANTOM based on Linux/Kali?

Yes. T‑PHANTOM OS is developed on top of Linux and uses upstream components from the Debian/Kali and KDE ecosystems. It does not claim authorship over those upstream projects or third-party tools. See `NOTICE.md` for attribution and licensing guidance.

## Where should bugs be reported?

Normal bugs can be reported through GitHub Issues. Security vulnerabilities should be reported privately according to `SECURITY.md`.

## What is the official contact?

**talal@talalsuhaimi.com**
