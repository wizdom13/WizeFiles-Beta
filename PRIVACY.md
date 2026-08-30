# Beta Testing Privacy Information

This document explains privacy expectations for participation through this public GitHub repository. The WizeFiles application's full privacy policy, when published, remains authoritative for app behavior.

## Public GitHub activity

Issues, discussions, comments, usernames, screenshots, and attachments posted here are generally public. GitHub processes this activity under its own terms and privacy policy.

Do not publish:

- Passwords, tokens, OAuth codes, cookies, or cloud configuration files
- Server addresses, usernames, account names, or private network details
- Private filenames, folder structures, document contents, or thumbnails
- Vault contents, encryption material, biometric information, or recovery keys
- APK/AAB signing keys, keystores, key-store passwords, or private certificates
- Private APK/APKS/APKM/XAPK files, OBB expansion data, package inventories, signer details, or installer screenshots that expose private applications
- Google Play purchase tokens, receipts, signed license documents, or installation identifiers
- Unredacted logs, crash reports, screenshots, or screen recordings
- Device identifiers that are not necessary for diagnosis

## Diagnostic information

WizeFiles maintainers may ask for the app version, Android version, device model, storage/provider type, reproduction steps, and sanitized diagnostics. Provide only the minimum information needed to reproduce the issue.

Version 0.7.0 can capture crash reports locally on the device. WizeFiles does not automatically upload these reports. A report leaves the device only when the tester explicitly chooses to share it through an Android share target. Review and sanitize every report before sharing because it may contain filenames, paths, provider details, device information, or recent application state.

Use placeholders such as `[ACCOUNT]`, `[SERVER]`, `[PRIVATE_PATH]`, `[SIGNING_KEY_REMOVED]`, and `[TOKEN_REMOVED]`. Signing and purchase reports should describe the key-store type, signature schemes, product type, and error state without attaching secrets, purchase evidence, or complete signed-license payloads. If a report cannot be safely sanitized, do not post it publicly.

## Security reports

Security vulnerabilities must be reported privately according to [SECURITY.md](SECURITY.md).

## Removing information

If sensitive information is accidentally published, edit or delete it immediately where possible and notify the maintainers. Public Git history, notifications, caches, or third-party archives may retain copies, so prevention is essential.
