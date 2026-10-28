# Windows Build 61

## Display acceptance update - October 28, 2026

The user confirmed that the desktop fills the viewing device and the Cintiq returns normally after disconnecting on Build 61. The viewing device was not identified in that response; this is one confirmed end-to-end result, not separate acceptance for both iPad and Surface.

Build 61 is now offered by the Windows preview update feed using the previously verified installer and SHA-256. No binaries were changed for this promotion. The release remains a development prerelease.

The original ZIP instructions and verification reports are historical snapshots from preparation/installation. Their pending acceptance and feed-Build-60 fields are superseded by this update. Remaining tests include repeated reconnects, portrait/landscape, guarded fault recovery, monitor changes, clean-install driver setup and ARM64 incoming display capability. Tablet Pro Touch/UIPI work is still separate.

---

Original publication record follows; the dated update above supersedes its pending-test/feed status.

Crystal Build 61 improves preparation and recovery of the virtual screen used to fit another device's display.

**Test release:** installed and verified on the ASUS on October 28, 2026. End-to-end connect/disconnect display acceptance for this build is still pending. The automatic-update feed remains on Build 60 while that check is completed.

Download **Crystal-Build-61-Setup.zip**, extract it, and run **Crystal-Build-61-Setup.exe**. The same installer chooses native x64 for the ASUS or ARM64 for the Surface automatically. The EXE is also available directly. These public downloads do not require a GitHub account.

- Cleans up a leftover, uniquely verified Crystal-owned virtual screen before a new matching session, using the current physical desktop as the recovery baseline.
- Waits when an earlier connection or either of its screen-recovery processes is still using the display. A stopped primary process does not allow a new session to override a surviving backup.
- Preserves physical screen position, orientation, resolution, refresh rate and HDR during verified cleanup; refuses preparation if ownership or recovery is uncertain.
- Retries a temporarily busy preparation safely. An idle backup failure can be retried only after the physical desktop has been positively verified as recovered.
- Checks that the native display recovery component matches the installer, alongside the existing checks for Extend and Mirror.

Installer version **0.61.0**, application **Build 61**, internal Setup Preview 13. Stop active sessions before installing. Setup closes and reopens Crystal and preserves saved identity, approvals and access choices. Windows may request approval.

**Verified:** native x64/ARM64 builds; 140 installer, 203 companion, 28 identity, 62 display-settings, 22 simulated recovery-transaction, 41 guard-policy and 17 actual cross-process coordination checks; packaged fresh start/restart with disposable state. The ASUS installation matches the package, preserves saved approvals, has both recovery processes ready, and leaves the Cintiq at 3840 x 2160, 120 Hz with HDR.

**Still to test:** physical screen handoff and restoration after connecting/disconnecting this build, portrait/landscape switching, guarded failure recovery and clean-install display-driver setup. ARM64 incoming display-driver support is not established by the ARM64 client build. This release does not change Tablet Pro Touch input behavior, the streaming/network protocol, or the Apple app.

The ZIPs retain their original preparation-time START-HERE/VERIFICATION files, which say the candidate was not yet installed or published. That is historical evidence, not the current release status. The separate **INSTALLATION-VERIFICATION.json** and this release page record the later ASUS installation; they do not claim physical reconnect acceptance.

**Source:** use **Crystal-Build-61-Source.zip** for the matching source baseline, focused patch, new files, tests, build order and upstream license notices. GitHub's automatically generated Source code ZIP contains this distribution repository, not the application source. Keep all included license notices. This is an unsigned development preview, not a production release or an iOS/iPadOS installer.
