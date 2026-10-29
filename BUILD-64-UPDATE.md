# Crystal Build 64 — compact pairing and touch recovery

Install `Crystal-Build-64-Setup.exe`, or extract it from the ZIP. The installer automatically selects the native Windows x64 or ARM64 viewing app and keeps saved computer identities, approvals and settings. Downloads are public and require no GitHub sign-in.

- Smaller signed pairing QR with the Prism show/hide eye. New linking asks for one approval on the computer being used, with no separate PIN flow.
- Compact computer tiles show model/type and computer name. Phones and iPads remain approved viewing devices but are excluded from the Use list.
- Native touch routing and the narrowly scoped Artist Pad touch preview.
- Display recovery retains the actual physical-screen layout and retries temporary Windows display-access failures.

The ASUS's local Build 64 components are working: the user confirmed Artist Pad touch/SPT, Cintiq restoration after disconnect, and improved Wi-Fi smoothness. Installer payload/identity/startup checks and QR/handshake tests are supplied in `VERIFICATION.json`. Sustained 120 FPS is not independently proven.

**Preview limits:** The Surface app/transport/decoder are native ARM64. Its desktop-sharing engine uses Windows 11 x64 compatibility in this build and incoming ARM sharing needs physical validation. The optional protected-touch helper is x64, supports the tested Artist Pad version and requires explicit Windows approval after each desktop-engine restart; it is not an automatic elevated service. New compact QR scans on Apple need Bassem's matching Apple build. Existing approved connections are retained. A complete physical new-device single-approval test remains pending.

The matching source archive includes the current Windows source, dependency pins/build instructions and Apple integration reference. No live keys, saved approvals or pairing links are included. This remains an unsigned development prerelease.
