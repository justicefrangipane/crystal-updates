## Update availability - October 28, 2026

Build 63 is now offered by Crystal's Windows preview update checker for x64 and ARM64, at the user's request. The public installer downloads inside current Crystal versions without a GitHub sign-in. The ASUS has Build 63 installed and its incoming connection service is ready; saved device identity and approvals were preserved.

This remains a development preview. Automated QR decoding and UI checks passed; physical camera scanning and sustained Surface 120 FPS still need device testing. Feed promotion is not a claim that those tests passed. The existing Build 61 display recovery safeguards are unchanged. Earlier publication-time notes below are historical; this update supersedes their manual-download-only, feed-Build-61 and not-yet-installed status.

---

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
