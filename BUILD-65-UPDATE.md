# Crystal Build 65 — automatic update checks

Crystal now checks for updates when its window opens or is restored, including the QR-based linked-computers home screen. When a newer release is available, the orange download icon appears beside Settings. Click it to download with progress, then choose when to install.

Window-open checks refresh the release information instead of waiting for the six-hour background interval. Rapid repeated window actions are throttled for one minute. Checks run in the background and honor the existing automatic-check preference.

**This is a development preview. Email registration, the timed free trial and purchases are not enabled.** It is not the finished trial installer. No payment information is collected or charge made.

The installer automatically selects the x64 or ARM64 viewing app and preserves saved identities and approvals. Build 64's connection transport, desktop engine, touch helper and display recovery binaries are retained. On Windows 11 ARM, the viewing app and transport are native; the desktop-sharing engine uses x64 compatibility. Incoming ARM sharing still needs physical testing.

The optional protected Artist Pad touch helper still requires separate local approval after the desktop engine restarts. This release does not update Apple apps, introduce a new pairing protocol or change monitor switching behavior.

Validation: automatic-check backend and UI tests, x64/ARM64 compilation, installer payload checks, architecture selection, and disposable-profile startup/restart. See VERIFICATION.json for exact results and physical-device limits. Publishing does not install the update on the ASUS.

Use the specifically named `Crystal-Build-65-Source.zip` for the matching source and build instructions. GitHub's automatically generated source ZIP contains only this distribution repository. This is an unsigned preview.
