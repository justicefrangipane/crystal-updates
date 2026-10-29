# Crystal preview updates

**Current Windows preview: [Build 64](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-64)** — compact pairing QR, one shared-computer approval, model/name tiles, touch routing and display recovery. [Release details](BUILD-64-UPDATE.md).

Download the EXE or ZIP from the release, or use Check for updates in Crystal on the Surface. No GitHub sign-in is required. Setup selects the native x64 or ARM64 viewing app and preserves saved approvals.

Windows 11 ARM uses an x64 desktop-sharing component in this preview; the viewing app, transport and recovery guard remain native ARM64. Incoming ARM sharing needs physical validation. Apple compact QR scans require Bassem's corresponding update; existing approved connections remain valid.

Use the specifically named `Crystal-Build-64-Source.zip` for matching application source and build instructions; GitHub's automatic source ZIP contains only this distribution repository. Preserve upstream license notices.

`preview.json` is schema 1 and includes the exact installer URL, byte length and SHA-256. Promotion occurs after anonymous asset verification. Crystal contains no GitHub account token. This is an unsigned development preview; public downloads do not publish device identities, approvals or desktop content.

[Previous Build 63](BUILD-63-UPDATE.md) · [Build 61 recovery evidence](BUILD-61-UPDATE.md)
