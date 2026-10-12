# Crystal update metadata

This repository contains only Crystal's Windows preview update information.
Source code, installers, device identities, and credentials do not belong here.

Downloads are in the private [Crystal project](https://github.com/justicefrangipane/crystal/releases).
You must be signed in to GitHub with access to that project to download a preview.

Crystal Build 48 and later check `preview.json`. They display an orange update icon
beside Settings only when a compatible build is newer than the installed one.
The icon opens release information; it never installs software automatically.

## Publishing a Windows preview

1. Compile and validate native x64 and ARM64 clients and the universal installer.
2. Publish the matching `build-N` release in the private Crystal project. Upload
   the tested installer ZIP, corresponding source, verification notes and SHA-256
   checksums. Verify the uploaded asset names, sizes and hashes.
3. Only after the release is available, change `build` and `release_url` together
   in `preview.json`. Keep `schema: 1`, `product: Crystal`, `channel: preview`,
   `platform: windows`, and the architectures actually included in the installer.
4. Run Crystal Settings > App > Check for updates and the native live-feed test.
   Verify an older build offers the release and the current build says up to date.

Never announce a placeholder or test build in the production feed. Use local
fixtures for tests. To withdraw a broken release, point the feed to the most
recent usable build; Crystal does not force a downgrade.

## Behavior and limits

Automatic checks run while the home window is visible and active, with a six-hour
interval after success and a thirty-minute retry after failure. Settings includes
a manual check and an automatic-check switch. Update metadata is at most 64 KiB;
the request has a 20-second timeout. A verified result is cached for up to seven
days across restarts. Errors do not imply that the app is up to date.

The request sends no Crystal account, device identity or pairing credentials.
GitHub necessarily receives the public internet address and ordinary HTTP request
information. The feed is protected by HTTPS and GitHub repository access control;
it is not cryptographically signed. The client accepts only the exact Crystal
release URL for that build and never executes content from the feed. A future
automatic installer must add signature verification before downloading/executing.

Do not include Apple build numbers in this Windows feed. Apple distribution and
update behavior require a separate implementation by the Apple team.
