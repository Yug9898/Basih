# Basih downloads

Mac release **1.0002.00.36** supports **M1-or-later Macs running macOS 26 or later**. The download contains the native My Basih app. Intel Macs, older macOS versions, the legacy app and Windows are not supported by this release.

[Download Basih for Mac](https://github.com/Yug9898/Basih/raw/refs/heads/main/Basih-for-Friend.zip)

Unzip and double-click **Install Basih.command**. The installer checks your Mac and macOS before replacing an app. Existing local entries, People balances, backups and Keychain credentials stay on your Mac. Existing supported installations can upgrade to My Basih.

This update:

- Brings the tested native Review, History, reporting, split selection and account controls to the regular app, preserving glass styling and your appearance preferences.
- Adds **Settle** to clear a person's balance without a bank payment or deleting the person. Connected people must both agree; both apps must be on this version or later. Changes to the reviewed entries invalidate a pending settlement.
- Keeps original spending and bank movements when settling or removing people. Account removal offers history preservation or a balance transfer to Cash.
- Adds force-click account comparison and confirmed deletion in Raw mode. Preserved historical records remain read-only.
- Identifies the specific Plaid connection needing renewed sign-in and offers Reconnect. A bank requiring sign-in no longer prevents healthy connections from loading.
- Reduces repeated Review preparation and fixes a cancelled-load navigation race. Offline People no longer continually prompts for sign-in.


To restore a backup, open **Settings → Backups → Choose backup…**, select the SQLite backup and confirm its passcode. A safety backup is created first; the selected original is retained. A backup moved to another Mac may require reconnecting bank or merchant-search credentials.

These apps are ad-hoc signed, not notarized. macOS may require approval in Privacy & Security on first launch. Touch ID may be unavailable without distribution provisioning; passcode unlock is supported.

Downloads contain no personal ledgers, backups or private API keys. Older artifacts remaining in this repository are historical downloads, not supported current releases.
