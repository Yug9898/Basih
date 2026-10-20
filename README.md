# Basih downloads

Mac update **1.0002.00.32** keeps normal bank-sync downloads from blocking local balances and saves, alongside the report, retry, and financial-integrity fixes. Existing records, backups and Keychain credentials stay on each user's Mac; the download contains no personal or test data.

- Manual and startup bank sync fetch provider data and optional merchant suggestions outside the live ledger lock. Local reads and saves can proceed while those services respond.
- If records, mappings, authorization or the database change during a download, the result is discarded and sync must be retried. Overlapping syncs cannot apply the same captured state twice.
- Initial bank connection setup/disconnection retain their existing serialization; large-history pagination remains future work.
- Custom spending categories now appear in Yearly reports and report totals, including refunds and viewer-hidden categories.
- Native new-entry retries reuse a durable command ID after a lost reply, preventing duplicate financial entries. A completed save allows a new intentional identical entry. This retry protection does not yet apply to the compatibility web interface.
- Repeated automatic loads for the same native page and data generation are suppressed.
- Adding a pending bank record refreshes native Activity and account balances immediately, without restarting the app. Older refresh responses cannot replace newer page data.
- The native Review badge includes waiting bank records that have not been added to Activity. Pending records already added are not counted again.
- Existing unknown People openings remain unknown. Deleting a local person retains their balance, notes and financial history, including people with recorded entries.
- Bank linking protects each account movement and its exact amount. Editing or deleting splits releases invalid repayment allocations while preserving the actual payment and revision history.
- Unchanged pending splits post in place. Changed allocated amounts remain in Review for reconciliation without blocking unrelated sync.
- Shared-account networking remains disabled in personal and Friends editions. Counterparty unlink approval applies to the isolated simulator only.

[Download Basih for Mac](https://github.com/Yug9898/Basih/raw/refs/heads/main/Basih-for-Friend.zip) · [Download Basih for Windows](https://github.com/Yug9898/Basih/raw/refs/heads/main/Basih-for-Windows.zip)

Mac release **1.0002.00.32**: unzip and double-click **Install Basih.command**. Existing users can choose **Settings → Updates → Update Basih** in their old app.

- Activity entries support inline hard-click editing with expanding Save, Cancel and Delete controls. This release uses the normal app interface; TESTUI/TESTCOM shared-account experiments are disabled.

- New native users start with a small orange glass panel. Choose New user for the five-page welcome guide; Restore backup appears when local backups are found. Profile creation happens with Enter app on the final page. Successful restoration opens Home.
- Apple Silicon Macs on macOS 26 or later receive **My Basih**, with the native SwiftUI interface and Liquid Glass.
- Earlier supported Apple Silicon Macs (macOS 13–25) receive the compatible **Basih** interface.
- The installer verifies the new app before replacing the old Desktop copy. Existing **Basih Shared** records and backups stay in Application Support. A legacy **Basih** data folder is copied only if Basih Shared does not already exist.
- To retrieve a different backup, open **Settings → Backups → Choose backup…**, select the SQLite backup in Finder, enter its passcode and confirm. A safety backup is created before restoration; the original selected file is retained.
- Credentials stay in the Mac’s Keychain. macOS may request access again; a backup moved to another Mac may require reconnecting Plaid/Tavily.

On macOS 26 or later, Home, Activity, People, Review, Raw mode, History, Analysis, Settings, statement review, and Assistant use native SwiftUI. The top Add Entry button opens the native entry form. The Assistant gives contextual hover explanations, including weekly, monthly and yearly spending, bank-review guidance, and possible-duplicate clues; duplicate clues are suggestions only and never change or link entries automatically. Older supported macOS versions keep the compatible Basih interface. Touch ID may be unavailable without distribution provisioning; passcode unlock is supported. These Mac apps are ad-hoc signed, not notarized, so macOS may require you to allow the app in Privacy & Security on first launch.

Windows: unzip, then double-click **Install Basih.cmd**. This Mac release does not change the Windows download.

Downloads contain no personal ledgers, backups or API keys. Your financial records are stored locally on your computer.

