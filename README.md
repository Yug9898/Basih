# Basih downloads

Mac release **1.0002.00.33** supports **M1-or-later Macs running macOS 26 or later**. The download contains only the native My Basih app. Intel Macs, older macOS versions, the legacy app and Windows are no longer supported release targets.

[Download Basih for Mac](https://github.com/Yug9898/Basih/raw/refs/heads/main/Basih-for-Friend.zip)

Unzip and double-click **Install Basih.command**. The installer checks your Mac and macOS before replacing an app. Existing Basih Shared records, backups and Keychain credentials stay on your Mac. Existing Basih.app installations on supported Macs can upgrade to My Basih; the older app is no longer included.

This update:

- Home rejects stale balance refreshes and prevents delayed responses from undoing a lock.
- History groups People records, statements and bank entries into collapsible months, newest first.
- Deleting a person removes their record, notes and balance. Their split shares become your personal spending. Bank movements and other people's shares and settlements remain unchanged. Original transaction revisions remain; no new person archive is created.
- If a save's result is unknown, changing its details cannot silently create another entry. **Resolve previous save** safely retries the original details and closes the current draft without submitting the changes.
- Manual and startup bank sync fetch bank data and optional merchant suggestions outside the live ledger lock. Concurrent edits, mapping changes, restores or completed syncs discard stale downloads safely.
- Includes the pending-entry Activity refresh, waiting-entry Review badge, custom-category report totals and earlier financial-integrity fixes.

Shared-account networking remains disabled in My Basih and Friends. In the isolated shared simulator, a linked person must approve unlinking before deletion. Initial bank connection setup/disconnection retain their existing serialization.

To restore a backup, open **Settings → Backups → Choose backup…**, select the SQLite backup and confirm its passcode. A safety backup is created first; the selected original is retained. A backup moved to another Mac may require reconnecting bank or merchant-search credentials.

These apps are ad-hoc signed, not notarized. macOS may require approval in Privacy & Security on first launch. Touch ID may be unavailable without distribution provisioning; passcode unlock is supported.

Downloads contain no personal ledgers, backups or API keys. Older artifacts remaining in this repository are historical downloads, not supported current releases.
