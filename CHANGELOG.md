# Changelog

This file summarizes public WizeFiles Beta releases. Detailed notes, APKs, and SHA-256 checksums are published on the [Releases](../../releases) page.

## Unreleased

No unreleased changes are documented yet.

## Version 0.6.1 — 2026-08-04

### What changed

- Added direct WizeFiles-to-WizeFiles Nearby Transfer for files and complete folders using Google Play services Nearby Connections.
- Added explicit two-sided authentication: the receiver approves the request and displays a one-time QR that the sender must scan. There is no numeric-code fallback.
- Added copy-only sending, two-minute user-initiated receiver visibility, and a fresh 60-second QR for every initial or resumed connection.
- Integrated nearby send and receive jobs with Transfer Center progress, speed, ETA, pause, resume, cancellation, retry, and recoverable interrupted sessions.
- Added resumable streaming with durable 4 MiB checkpoints, hidden partial files, conflict handling, storage checks, and path-traversal protection.

### Please test

- Connect two WizeFiles devices, approve the receiver, scan the QR, and transfer individual files and nested folders.
- Try a wrong or expired QR, cancel scanning, and confirm that reconnecting or resuming requires a fresh QR.
- Pause, resume, cancel, interrupt, and reconnect transfers from both devices and from Transfer Center.
- Test local storage, SD card, SAF, cloud, SMB, FTP/FTPS, SFTP, and WebDAV sources where available.
- Test low-storage conditions, existing destination conflicts, screen-off behavior, and both large files and many small files.

### Known limitations

- Nearby Transfer works only between two WizeFiles devices and does not interoperate with Android Quick Share.
- Google Play services is required. Google Code Scanner may need internet access once to prepare its scanning module; subsequent scans can work offline.
- Version 0.6.1 supports one sender and one receiver per session. Receiving is never always-on and must be started by the user.
- Sending always copies and never removes the sender's source files.
- Beta builds expire 30 days after compilation.

### Installation notes

- Version 0.6.1 updates an installed WizeFiles Beta 0.6.0 build in place when both builds use the same beta signing key.
- WizeFiles Beta uses a separate application ID from the future stable app, so their app data remains separate.
- Back up important files and begin testing with data you can recover.

### Integrity

- APK: `WizeFiles_v0.6.1_beta.apk`
- SHA-256: `2bf581cc2ad7e5ebc6b9ac4ecd7e15127bd3dbb7f9f8904e5cf55e976ac62e11`
- Release: [WizeFiles v0.6.1 Beta](../../releases/tag/v0.6.1)

## Version 0.6.0 — 2026-08-03

### What changed

- Published the first public WizeFiles beta.
- Added multiple tabs, adaptive dual-pane browsing, drag-and-drop between panes, desktop keyboard shortcuts, and mouse context menus.
- Added a persistent Transfer Center with pause, resume, retry, history, recovery, speed, and ETA.
- Added folder synchronization, scheduled jobs, PC/browser access, and local network sharing.
- Added broad cloud and network storage support, including rclone cloud accounts, SMB, FTP/FTPS, SFTP, WebDAV, and S3.
- Added indexed instant search, advanced batch rename, duplicate detection, storage cleanup, and a visual disk map.

### Please test

- Local, SD card, USB, SAF, cloud, and network browsing and file operations.
- Multi-tab and dual-pane navigation, drag-and-drop, keyboard shortcuts, and conflict prompts.
- Transfer Center recovery, synchronization, scheduled jobs, and PC/browser access.
- Search indexing, batch rename previews, archives, storage cleanup, and disk analysis.

### Known limitations

- Direct nearby phone-to-phone transfer was not included in 0.6.0; update to 0.6.1 to test it.
- Editing archive contents in place and the installed-app manager/APK backup remain planned features.
- Beta builds expire 30 days after compilation.

### Installation notes

- WizeFiles Beta is a prerelease. Back up important files and test initially with recoverable data.
- The beta application can be installed separately from the future stable app, and each keeps separate app data.

### Integrity

- APK: `WizeFiles_v0.6.0_beta.apk`
- SHA-256: `70817394cb18696ebf0a08f48c508dfe35961a76df605fb326e3a2c000742b78`
- Release: [WizeFiles v0.6.0 Beta](../../releases/tag/v0.6.0)
