# Crystal preview updates

**Current preview:** [Crystal Build 61](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-61) adds display recovery safeguards. The user confirmed screen fit and Cintiq restoration after disconnecting. Build 61 is now offered in Crystal. [Details and remaining tests](BUILD-61-UPDATE.md).

[Download Crystal Build 61 for Windows](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-61).

This public repository hosts the update feed, preview installers and matching release source. No GitHub account is required to download them. Crystal selects native x64 or ARM64 during installation.

Download `Crystal-Build-61-Setup.zip`, extract it, and run the EXE. Build 61 adds display recovery safeguards and retains service recovery and direct downloads with progress from Build 60. Earlier versions can install this preview manually.

Source is provided in the specifically named `Crystal-Build-61-Source.zip` release asset, with its baseline, patches, build instructions and upstream notices. GitHub's automatic source archives contain only this distribution repository. Retain all applicable upstream license notices.

`preview.json` remains schema 1. Newer clients also read the exact installer URL, byte length and SHA-256. The feed is updated only after release assets are verified. Crystal never contains a GitHub account token.

Development prerelease. Device approval is still required for remote access; making downloads public does not publish device keys, approvals or desktops.
