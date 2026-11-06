# Crystal Windows preview

[Download Build 82](https://github.com/justicefrangipane/crystal-updates/releases/tag/build-82)


After installing a new version, Crystal shows a **Whatâ€™s new** popup once with
that version's additions and improvements. It waits for an active home screen,
shared controls to finish, and account or other dialogs to close. Reopening the
app, reinstalling the same version or rolling back does not repeat the notice.

Open **Settings â†’ App â†’ Whatâ€™s new**, or choose **Whatâ€™s new** in the update
window, for the full included history. Notes work offline, show the installed
build and release date, and use short Added, Improved, Fixed and Good to know
sections. The body scrolls while Close stays visible in small windows. The
initial history covers public Windows previews from Build 70 onward; Build 80
summarizes the unpublished local Builds 76â€“79.

Both Windows x64 and ARM64 clients compiled. Forty-two updater/history checks,
six focused QML checks at each of 100% and 150% scaling, and 175 installer checks
passed. The QML checks use the actual bundled notes and cover manual access,
once-only presentation, deferral behind account/update dialogs and shared
controls, full-history access, and compact dark/light layouts. This release has
not been installed on the ASUS or physically run on the Surface during this
work. Existing account, companion, input, transport and display-recovery
components are retained byte-for-byte from Build 81.

A source handoff adds the same offline history and automatic popup to Bassem's
latest shared iPhone/iPad and Mac Catalyst code. Its patch applies and resource
membership checks pass, but Xcode compilation and Apple device acceptance are
still required. This Windows release does not install or publish an Apple app.

Known issue: Microsoft may still quarantine confirmation emails; the separate
support investigation remains open. First use offers a three-day no-email
trial; confirming email extends the same trial to seven days total. Updates do
not reset trial dates. Purchases remain unavailable. This is an unsigned
development preview, not a Microsoft Store release. Incoming desktop sharing
on Windows ARM64 still uses x64 compatibility and remains experimental.

Use the explicit Crystal-Build-82-Source.zip for matching source and notices.
No website download, email settings, installed drivers or live display settings
were changed by publishing this release.
