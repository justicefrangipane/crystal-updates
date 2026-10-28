# Crystal Build 63 â€” Prism pairing and Home 120 FPS

The centered Prism eye shows or hides the pairing code. Tap outside the eye to
enlarge the visible code. Hidden codes stay hidden when invitations refresh;
existing approvals and incoming-access choices are preserved.

Includes Home 120 FPS / 50 Mbps, a separate 30/60/120 FPS selector, and Travel
30 FPS / 5 Mbps. Screen shape, resolution percentage, HDR and touch settings
are kept. Reconnect after changing picture settings. On Surface, select
120 Hz in Windows and start with 75% resolution.

The installer selects x64 or ARM64 automatically. Matching source and build
instructions are included. No transport or display-recovery binaries changed.

Validation: both architectures compile; installer, saved-identity, startup and
settings tests pass. The actual pairing UI is exercised with disposable local
devices, including hide/reveal, renewal, approval and revocation. The real
rendered QR is checked by an independent decoder at normal and high-DPI scale.

This is a **manual test release**. Physical Apple camera scanning, Surface ARM64
runtime behavior and sustained 120 FPS still need testing. Build 63 has not
been installed on ASUS by this publication. The automatic update feed remains
on Build 61, whose screen fit and Cintiq restoration were user-confirmed.

[Bassem's integration checklist](https://github.com/justicefrangipane/crystal/blob/main/handoffs/BUILD-63-BASSEM.md).
