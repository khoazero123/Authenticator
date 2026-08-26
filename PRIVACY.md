# Privacy Policy — Authenticator OTP

**Last updated:** 2026-08-26

This privacy policy applies to the browser extension **Authenticator OTP** (the “Extension”), a fork of [Authenticator Extension](https://github.com/Authenticator-Extension/Authenticator).

## Single purpose

Authenticator OTP generates two-factor authentication (TOTP/HOTP) codes in your browser. You can add accounts (QR code or secret), view codes, copy or autofill them, optionally lock the vault with a passphrase, and back up or restore account data.

## Data we collect

**We do not collect, transmit, or sell your personal data.**

The Extension’s developer does not operate a backend that receives your OTP secrets, account labels, passwords, browsing history, or analytics.

## Data stored on your device

The Extension stores data locally in your browser (`chrome.storage` local and/or sync), including:

- OTP account information (secrets, issuer/account labels, and related settings)
- Optional passphrase-protected encryption of stored secrets
- Extension preferences (for example autolock, backup options, UI settings)

Browser sync storage, if enabled by you, is handled by your browser/account provider (for example Chrome Sync), not by us.

## Optional cloud backup

If you choose to enable backup to a third-party service (such as Dropbox, Google Drive, or OneDrive), account data you export is sent **only** to that service under **your** account, using OAuth permissions you grant.

- We do not receive your backup files.
- Those services are governed by their own privacy policies.
- You can disable cloud backup and revoke related permissions at any time in the Extension or browser settings.

## Permissions

The Extension requests only permissions needed for its features:

| Permission | Purpose |
| --- | --- |
| `activeTab` | Scan QR codes / capture the current tab when you request it |
| `storage` | Store account data and settings in the browser |
| `identity` | Optional OAuth sign-in for cloud backup providers |
| `alarms` | Optional auto-lock timer for the vault |
| `scripting` | Inject helpers for QR scanning and optional autofill on the current page |
| `clipboardWrite` (optional) | Copy an OTP code when you choose to copy |
| `contextMenus` (optional) | Add Extension actions to the browser context menu |

Host permissions for backup providers or clock sync are requested only when you enable those features.

## Data sharing

We do not share Extension data with third parties, except when **you** explicitly use optional backup integrations, in which case data goes to the provider you selected.

## Security

- Secrets can be encrypted with a passphrase you set (client-side).
- Keep backups and your passphrase secure. Anyone with an unencrypted backup or your passphrase may access your OTP secrets.
- Losing your passphrase may make encrypted data unrecoverable.

## Children’s privacy

The Extension is not directed at children and is not intended for users under 13.

## Changes

We may update this policy from time to time. The “Last updated” date at the top will change when we do. Continued use of the Extension after updates means you accept the revised policy.

## Contact

Questions about this privacy policy:

- GitHub: [https://github.com/khoazero123/Authenticator](https://github.com/khoazero123/Authenticator)
- Open an issue on that repository

## Open source

Source code is available at [https://github.com/khoazero123/Authenticator](https://github.com/khoazero123/Authenticator). You can review how data is handled in the code.
