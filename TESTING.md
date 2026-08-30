# WizeFiles Beta Testing Guide

Thank you for helping test WizeFiles. Good reports describe one problem clearly, make it reproducible, and avoid exposing private data.

## Safety first

- Back up important files before testing copy, move, rename, delete, archive, extraction, synchronization, package installation, secure shred, or vault features.
- Start with disposable test data.
- Do not make a beta installation the only location of important data.
- Read the release notes for migration, signing, and stable/beta coexistence information.
- Confirm the destination after every destructive or cross-storage operation.
- Never share credentials, tokens, recovery keys, private documents, complete rclone configuration files, or unredacted logs.

## Recommended test cycle

1. Record the beta version and build number from **Settings → About**.
2. Record the Android version and exact device model.
3. Read the release's testing focus and [known issues](KNOWN_ISSUES.md).
4. Reproduce the workflow with a small test file.
5. Repeat it once after restarting WizeFiles.
6. If safe, repeat on another storage type or network.
7. Submit one issue per distinct defect.

## High-value areas

### Launch, update, and Beta Pro state

- Confirm a newly installed or updated minified Beta reaches the browser without a startup crash.
- Open **About → WizeFiles Pro** and verify the valid Beta reports active Pro access.
- Confirm Beta shows no prices, purchase offers, restore checkout, or route into Google Play Billing.
- Exercise dual-pane, sync/schedules, package signing, archive mutation, batch App Manager actions, additional connections/vaults, rclone power-user setup, root, and local-server entry points while Beta Pro is active.
- Verify existing files, vaults, connections, and Transfer Center history remain readable after restarts and configuration changes.

### Local and removable storage

- Internal storage and app-accessible folders
- Storage Access Framework folders
- SD cards and USB drives
- Permission loss after restart or device reboot
- Copy, move, rename, delete, Trash Bin recovery, secure shred, and conflict handling

### Network and cloud

- FTP, SFTP, SMB, WebDAV, and S3
- Cloud-account connection and reconnection
- Upload, download, rename, delete, and remote-to-remote workflows
- Normal-tap opening and **Open with** behavior for remote text and document files
- Interrupted transfers and recovery
- Slow, unstable, or metered networks

### Navigation and productivity

- Multiple tabs
- Single-pane and dual-pane switching
- Independent pane navigation and selection
- Bottom selection actions for one file, one folder, multiple files, and mixed file/folder selections in both List and Grid layouts
- Back clearing selection before navigation and restoring pending Paste or picker panels
- Browser and Vault view/sort toolbar actions, localized item-count subtitles, icon tinting, and disabled states
- Browser and Vault floating action menus in this order: New File, New Folder, New Secure Folder, Connect Cloud Drive
- New File/New Folder dialogs: rounded shape, balanced field margins, validation, focus, keyboard insets, and cancellation
- Search and index refresh
- Batch rename preview and results
- Keyboard, mouse, tablet, foldable, and desktop-mode behavior

### Long-running operations

- Transfer Center state and progress
- Pause, resume, retry, and cancellation where available
- Process termination and restart recovery
- Folder synchronization and scheduled jobs
- Conflict, overwrite, and delete confirmations

### Archive modification

- Add files, deep folder trees, and empty folders to unencrypted ZIP, 7z, and TAR.XZ archives.
- Rename and delete individual entries and populated folders.
- Exercise Replace, Keep both, Skip, and Cancel conflict choices.
- Paste from local, SAF, SD card, USB, cloud, and network sources where available.
- Pause, cancel, or terminate WizeFiles during reconstruction and confirm the original archive remains valid.
- Test low-storage, remote-quota, disconnected-provider, corrupt-archive, Unicode-name, and case-collision conditions.
- Confirm encrypted, split, nested, signed, and unsupported archive formats stay read-only.

### App Manager and APK backup

- Verify All, User, System, and Disabled filters, search, sorting, and selection clearing/preservation.
- Verify Open, App Info, single uninstall, cancelled uninstall, and sequential multi-uninstall through Android's confirmation UI.
- Select a system app or a mixed selection containing one and confirm Uninstall is disabled.
- Select enabled apps, disabled apps, and mixed-state apps; confirm the context-aware Enable/Disable action and disabled state are correct.
- Back up and share a regular app as `.apk`; verify its filename and installability.
- Back up a split app as `.apks`; inspect `base.apk`, all splits, `metadata.json`, and SHA-256 checksums.
- Send backups to local, SAF, cloud, FTP/SFTP/SMB, and rclone destinations; verify Transfer Center progress, conflicts, cancellation, and no partial output.
- Confirm backups never claim to include application data, accounts, preferences, or private files.

### Built-in viewers and advanced formats

- Test image/video previews, background audio, PDF, EPUB/Kindle-family books, HTML/XHTML, MHTML, CHM, and MAFF from local, SAF, root, Vault, archive, network, and cloud sources.
- Test ICO/CUR, TIFF/BTF, TGA-family, and camera-RAW previews with valid, corrupt, oversized, truncated, and unsupported samples.
- Open TTF, OTF, variable-font, and TTC samples; verify family/style/weight metadata, editable specimen text, multilingual samples, and the 12–84 sp preview range.
- Verify common media stays on Media3 and specialist formats can fall back to LibVLC without loops; test notifications, lock screen, seek, audio focus, Bluetooth, and unplug-to-pause.
- Browse representative RAR/RAR5, CAB, ISO/UDF, WIM, DMG, filesystem, virtual-disk, and split-volume containers; confirm they remain read-only and extraction uses normal safety limits.
- Confirm DRM/encrypted Kindle content, outbound saved-web subresources, unsafe links, traversal paths, oversized expansion, and unsupported decoding fail safely with **Open with** available.

### Android package installation

- Install, update, reinstall, and downgrade disposable same-signer APKs; confirm ordinary installs use Android's confirmation UI.
- Open APKS, APKM, and XAPK containers and verify the selected ABI, density, locale, base, and feature splits match the device.
- Compare installed and incoming version codes, signing certificates, permissions, required features, and components before installation.
- Confirm a signer mismatch blocks ordinary replacement and is explained beside the version comparison.
- On a rooted test device, verify **Allow version downgrade** enables only an otherwise valid matching-signer downgrade.
- On a rooted Core Patch-compatible test device, verify **Allow signature mismatch (root/Core Patch)** requires separate risk confirmation and never claims that WizeFiles patches Android.
- Test valid and invalid XAPK OBB names, package/version mismatches, traversal paths, conflicts, low storage, destination denial, retry, rollback, and the **app installed, expansion files failed** result.
- Cancel, background, rotate, kill, and recreate the installer during inspection, review, Android confirmation, session commit, and OBB placement; confirm staged files and abandoned sessions are cleaned safely.
- Never use an irreplaceable installed app, application data, or OBB directory for initial installer tests.

### Android package signing and verification

- Sign APKs with v1, v2, v3, and v2/v3 plus detached v4; verify every requested scheme and signer certificate afterward.
- Import PKCS#12, JKS, and BKS keys and generate a password-protected PKCS#12 RSA key.
- Test local, SAF, root, archive, network, cloud, and Vault sources/destinations, keep-both conflicts, cancellation, process interruption, and password re-entry recovery.
- Test wrong passwords, missing aliases, malformed packages, tampered outputs, existing `.idsig` files, and attempts to overwrite the input.
- Test AAB upload-key signing/verification and APKS/XAPK/APKM workflows; verify every contained APK shares the intended signer and non-APK payloads remain unchanged.
- Never include private keys, keystores, passwords, certificates containing private identity data, or purchase tokens in a report.

### Appearance and content visuals

- Switch among all 12 icon shapes and confirm **Squircle** is the default.
- Verify shape previews remain clear in light, dark, black, and dynamic-color themes.
- Check built-in file/folder icons, image/video thumbnails, and APK artwork in List, Auto Grid, and manual grid-count layouts.
- Check the same shapes and responsive grid behavior in Browser, Vault, Storage Cleaner, and file-operation conflict previews.
- Change grid count and icon shape while content is visible, then scroll rapidly and confirm recycled cells do not show stale, clipped, or square backgrounds.
- Rotate, resize, enter split-screen, and change fold state where available; confirm Auto Grid recalculates from usable width while manual counts remain selected.
- On large phones and tablets, confirm icons are capped at a readable size and the grid uses the available space without excessive gaps.
- Verify video play badges and other overlays remain clear and are not clipped incorrectly.

### External media handoff

- Use **Open with** and **Edit with** for images and videos with compatible Android apps.
- Confirm writable edits can be saved back when the external app supports the provided URI.
- Verify media thumbnails and image/audio/video properties remain available after editor removal.
- Test the no-compatible-app case and confirm WizeFiles reports it without crashing.

### Local crash reports

- Confirm a captured report remains on the device until the user chooses a share target.
- Review the report before sharing and verify it can be cancelled without transmission.
- Sanitize filenames, paths, account/provider details, device identifiers, signing material, purchase data, and other private content.
- Confirm the app can reopen normally after the report is handled or dismissed.

### Trash Bin and secure shred

- Move disposable supported local files and folders to Trash Bin, restore them, and verify ordinary deletion remains recoverable.
- Securely shred separate disposable writable local targets and confirm the irreversible warning, explicit confirmation, completion result, and absence from Trash Bin.
- Confirm secure shred is unavailable for remote, SAF, archive, and mixed-provider selections.
- Interrupt a shred operation and confirm remaining items and partial outcomes are reported accurately.
- Remember that flash wear levelling, snapshots, backups, and synchronized copies prevent software overwrite from guaranteeing physical erasure.

### Analysis and security

- Duplicate detection
- Storage cleanup and visual disk analysis
- Archives and password prompts
- Vault lock/unlock and biometric behavior
- Root and Shizuku features on supported devices

## What makes a useful bug report

Include:

- Exact steps, beginning from a known screen
- Expected and actual results
- Frequency: always, intermittent, or happened once
- WizeFiles version/build
- Android version and device model
- Storage/provider type
- Whether restarting WizeFiles or the device changes the result
- A sanitized screenshot, screen recording, or diagnostic log when helpful

Replace private values with clear placeholders such as `[ACCOUNT]`, `[SERVER]`, `[PRIVATE_PATH]`, and `[TOKEN_REMOVED]`.

## Regression check

If a workflow worked in an earlier beta, name the last working version and the first broken version. This is especially valuable for storage permissions, database migrations, remote providers, and long-running operations.
