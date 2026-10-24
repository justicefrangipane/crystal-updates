# Windows Build 60

Crystal Build 60 keeps approved computers available and adds downloads directly inside Crystal.

Download **Crystal-Build-60-Setup.zip**, extract it, and run **Crystal-Build-60-Setup.exe**. The same installer selects native x64 for ASUS and ARM64 for Surface automatically. Alternatively download the EXE directly. No GitHub account is needed for these public preview files.

- Recovers the desktop connection service while Crystal is open and retries a stopped built-in connection using saved identity and approvals.
- With Allow access and Ready when I sign in enabled, the Windows recovery task can restore Crystal in the tray after an unexpected exit. Deliberately choosing Exit Crystal or turning access off still stops incoming connections.
- Replaces the update icon with a clear orange download symbol. Selecting it downloads inside Crystal with progress and cancellation. The installer is checked for the expected size and SHA-256, then Install update is a separate action.
- Preserves the existing display recovery components. This release does not introduce new display switching behavior or reset pairing permissions.

Installer version **0.60.0**, app identity **Build 60**, internal Setup Preview 12. Close active sessions before installation. The installer closes and reopens Crystal and preserves saved approvals. Windows may request setup approval. Older versions need this first update installed manually; the new in-app downloader handles subsequent published updates.

Validation: native x64 and ARM64 builds; 38 updater tests, 23 lifecycle checks, 136 installer checks, 199 companion checks and 28 connection identity checks; actual receiver stop/restart with disposable loopback state; packaged fresh-start/restart. The original VERIFICATION.json records preparation-time evidence, so its installed/published flags remain false. Live installation and GitHub download checks are recorded separately. Physical Surface and iPad confirmation for Build 60 remains pending.

**Source:** Crystal-Build-60-Source.zip contains the reconstructable source baseline, changes, tests and build instructions. Retain the included upstream license notices. GitHub's automatic Source code ZIP contains this distribution repository, not the complete application source. Use the specifically named Source.zip asset instead. This is an unsigned development preview, not an Apple app update or a production release.
