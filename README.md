# Crystal Windows preview

[Download Build 81](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-81)


Crystal now offers **Enable controller support** when this computer allows incoming connections and its ViGEm driver is missing. It explains the one-time Windows approval and uses **ViGEm** in Crystal's interface. An existing driver installed by Tablet Pro Gamepad or another app is reused.

Setup is optional. It is never launched during Crystal installation or startup. Selecting it briefly pauses connections and uses the existing display-recovery routine before Windows approval. Availability resumes afterward, including cancellation or a failed setup. A newer explicit Exit Crystal is respected. Setup does not reboot Windows or remove a shared driver. The original signed installer and required license are preserved; Windows controls the publisher text in its own approval window.

The driver package is pinned by SHA-256 and checked with Windows signature verification before launch. Crystal handles canceled approval, missing files, unknown driver state, failed installation and a required restart. An installer exit code alone does not establish success. Advanced options and copied connection details include the driver state.

Both Windows clients compile. Validation includes 110 controller-setup checks, 270 companion checks, 175 installer checks and the real home QML/loopback pairing/QR suite at 100% and 150% scaling. The new helper read the existing ASUS driver as ready without changing it. A clean-machine installation through the actual Windows approval prompt is still pending; simulated setup outcomes do not establish that physical result. Build 81 has not been installed on the ASUS or run on a Surface/iPad during this release work. The earlier Build 80 Surface screen-fit/touch/X-close acceptance is still awaiting completion.

Account enforcement, desktop capture, transport, protected touch and display-recovery components are retained from Build 80. The companion adds only the explicit controller-setup route. No Apple source or build is included. Windows ARM64 viewing/transport are native; incoming desktop sharing still uses x64 compatibility and is experimental.

**Known issue:** Microsoft can quarantine confirmation emails; support review remains open. First use offers three days without email; confirming email extends that trial to seven days total. Updating does not reset an expired trial. Purchases and automatic charges remain unavailable. This is an unsigned development preview, not a Microsoft Store release.

Use Crystal-Build-81-Source.zip for the matching source and notices; GitHub's automatic source archive is the distribution repository only. BUILD-81-BASSEM.md contains the Apple handoff. No website download or email-service configuration was changed in this release.
