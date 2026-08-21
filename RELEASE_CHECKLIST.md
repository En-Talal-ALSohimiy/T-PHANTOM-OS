# T‑PHANTOM OS Release Checklist

Use this checklist before publishing a public ISO.

## Identity

- [ ] User-facing OS name is T‑PHANTOM OS.
- [ ] Boot menu branding is correct.
- [ ] Installer branding is correct.
- [ ] Login screen branding is correct.
- [ ] Desktop wallpaper and identity are correct.
- [ ] Developer information opens successfully.

## Boot and install

- [ ] BIOS boot tested where supported.
- [ ] UEFI boot tested.
- [ ] Live session starts.
- [ ] Installer starts.
- [ ] Clean install completes.
- [ ] Installed system boots after ISO removal.
- [ ] Bootloader entries use T‑PHANTOM naming.

## Runtime

- [ ] `/etc/os-release` reviewed.
- [ ] Hostname reviewed.
- [ ] Root filesystem confirmed on installed disk.
- [ ] `systemctl --failed` reviewed.
- [ ] AppArmor check passed.
- [ ] nftables check passed.
- [ ] Arabic locale check passed.
- [ ] English locale check passed.
- [ ] Indexed tools reviewed for missing commands.

## Desktop

- [ ] SDDM login works.
- [ ] Plasma session starts.
- [ ] No unintended splash/branding appears.
- [ ] Default wallpaper is correct for a new user.
- [ ] Clipboard and common desktop functions tested.

## Physical hardware

- [ ] Graphics tested.
- [ ] Wi‑Fi tested.
- [ ] Ethernet tested.
- [ ] Audio tested.
- [ ] Storage controller tested.
- [ ] USB tested.
- [ ] Shutdown/restart tested.
- [ ] Suspend/resume tested where applicable.

## Artifact integrity

- [ ] Final ISO filename confirmed.
- [ ] Final ISO boots after last modification.
- [ ] SHA‑256 generated from the exact published ISO.
- [ ] `SHA256SUMS` matches the artifact.
- [ ] Downloaded mirror copy re-hashed and matched.

## Publication

- [ ] README matches actual validated behavior.
- [ ] CHANGELOG updated.
- [ ] Known limitations disclosed.
- [ ] Installation guide reviewed.
- [ ] Security contact valid.
- [ ] Third-party notices and licensing reviewed.

A release should not be described as fully qualified until the relevant unchecked items are completed or explicitly documented as known limitations.
