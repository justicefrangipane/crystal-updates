# Crystal preview updates

[Download Crystal Build 60 for Windows](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-60).

This public repository hosts the update feed, preview installers and matching release source. No GitHub account is required to download them. Crystal selects native x64 or ARM64 during installation.

Download `Crystal-Build-60-Setup.zip`, extract it, and run the EXE. Build 60 adds service recovery and direct downloads with progress inside Crystal. Earlier versions need this first installation performed manually.

Source is provided in the specifically named `Crystal-Build-60-Source.zip` release asset, with its baseline, patches, build instructions and upstream notices. GitHub's automatic source archives contain only this distribution repository. Retain all applicable upstream license notices.

`preview.json` remains schema 1. Newer clients also read the exact installer URL, byte length and SHA-256. The feed is updated only after release assets are verified. Crystal never contains a GitHub account token.

Development prerelease. Device approval is still required for remote access; making downloads public does not publish device keys, approvals or desktops.
