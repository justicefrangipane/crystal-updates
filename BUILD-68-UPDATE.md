# Crystal Build 68 — immediate pen preview

Build 68 adds a local pen-tip ring so you can see where the pen is without waiting for the streamed video. It is enabled by default on Windows. Your drawing app still supplies the actual ink; this is not predicted ink.

[Download the Windows installer](https://github.com/justicefrangipane/crystal-updates/releases/download/build-68/Crystal-Build-68-Setup.exe) · [Installer ZIP](https://github.com/justicefrangipane/crystal-updates/releases/download/build-68/Crystal-Build-68-Setup.zip) · [Matching source](https://github.com/justicefrangipane/crystal-updates/releases/download/build-68/Crystal-Build-68-Source.zip)

No GitHub sign-in is needed. The installer selects x64 or ARM64 automatically and preserves saved computer approvals. Install on both Windows computers, then reconnect. On the Surface, **Immediate pen preview** is on by default; changes to that setting take effect after reconnecting.

## Changes

- A small, hollow marker follows the latest pen position locally. It does not block taps, take focus, or alter pressure, tilt or touch delivery. It hides when the pen leaves, Crystal loses focus, or the pen is over Crystal's local stream controls.
- Local mouse-pointer discovery now finds the renamed Crystal desktop process and reconnects after that process restarts.
- The QR eye is centered in its button in both shown and hidden states.
- Connection failures distinguish secure-connection problems from a stopped or unresponsive desktop service. **Copy details** provides local diagnostic information; it is not uploaded automatically. A bounded readiness check offers a retry without discarding saved approvals.
- Includes the prepared capture-recovery changes and a corrected screen-mode settings lock check. Existing independent display guards are preserved.

## Verified and still to test

Automated checks passed: 143 installer, 213 companion, 28 identity, 18 connection recovery, 112 recovery UI/TLS, 13 cursor discovery and 38 native pen preview checks, plus input routing, preferences and isolated startup/restart. Both x64 and ARM64 viewing clients compiled.

**Physical-device pen feel and ARM64 installation acceptance remain pending.** Actual clicks and ink still depend on network and video latency. Display handoff/recovery acceptance also remains pending. The automatic update feed remains on Build 65 pending acceptance; Build 68 is available here for manual testing.

Artist Pad's optional elevated touch helper still requires local Windows approval after the desktop service restarts. This update does not bypass that requirement. On Windows 11 ARM, the viewer is native ARM64; incoming desktop sharing uses x64 compatibility and still needs physical validation.

This is an unsigned development preview. Email registration, timed trials and purchases remain disabled. No Apple app binary is included. Bassem's integration notes are included as `BUILD-68-BASSEM.md`.

Use **Crystal-Build-68-Source.zip** for the matching application source, build instructions and licenses. GitHub's automatically generated Source code archives contain only the distribution repository. Public package instructions and verification summaries omit private test-machine configuration; application, desktop-engine, transport and guard binaries are unchanged from the tested Build 68.
