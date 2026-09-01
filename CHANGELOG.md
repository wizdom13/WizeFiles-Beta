# Changelog

## Upcoming open-source transition

- Removed Google Play Billing, purchase and restore UI, signed purchase-license verification, Pro entitlements, and all Free/Pro feature limits from the development branch.
- Made every implemented capability available in every build without purchases, subscriptions, advertisements, or feature paywalls.
- Relicensed WizeFiles under the GNU General Public License version 3 (GPL-3.0-only).
- The published 0.7.0 Beta remains the current downloadable build until a newer GPL/open-feature beta is released.

This file summarizes public WizeFiles Beta releases. Detailed notes, APKs, and SHA-256 checksums are published on the [Releases](../../releases) page.

## Unreleased

No unreleased changes are documented yet.

## Version 0.7.0 — 2026-08-30

### What changed

- Added a WizeFiles-owned Android package installer for APK, APKS, APKM, and XAPK files.
- Added strict package, version, split, and signer verification with device-compatible ABI, density, and locale split selection.
- Added a review screen comparing installed and incoming versions, signing identities, permissions, features, and application components.
- Added normal Android-confirmed installation, root-gated downgrade, and a separately warned signature-mismatch option for devices already using Core Patch or a compatible system modification.
- Added validated XAPK OBB staging and destination checks, transactional placement, root fallback, rollback, retry, and honest partial-completion reporting.
- Added a TTF, OTF, and TTC Font Viewer with font metadata, editable specimen text, multilingual samples, and adjustable preview size.
- Added secure shred for supported writable local files and folders with one-pass zero overwrite, synchronization, and permanent deletion.
- Renamed Recycle Bin wording to Trash Bin and documented the distinction between recoverable deletion and irreversible shred.
- Polished the installer with the standard back arrow, Material 3 semantic change colors, an accessible vector options icon, readable signer warnings, and spaced actions.
- Expanded documentation for installer security, OBB limitations, Font Viewer behavior, secure-shred limitations, and public feature coverage.

### Please test

- Install, update, reinstall, and downgrade same-signer standalone APKs; verify Android confirmation appears for ordinary installs.
- Open APKS, APKM, and XAPK containers and confirm the selected ABI, density, and locale splits match the device.
- Compare installed and incoming version codes, signers, permissions, features, and components; confirm signer mismatch blocks ordinary replacement.
- On a rooted test device, verify downgrade requires explicit approval and signature mismatch additionally requires the separate Core Patch-compatible approval.
- Install a disposable XAPK containing valid OBB files; verify destination validation, successful placement, retry, rollback, and partial-completion reporting when storage access is unavailable.
- Open representative TTF, OTF, variable-font, and TTC samples and verify metadata, specimen editing, multilingual samples, and preview sizing.
- Test Trash Bin recovery and secure shred separately with disposable writable local files and folders; confirm unsupported remote, SAF, archive, and mixed-provider selections cannot be shredded.
- Rotate, resize, background, cancel, and recreate the installer at each stage and confirm no partial APK session or stale staged files remain.

### Known limitations

- AAB installation is not included; AAB signing and verification remain available.
- Multi-variant APKS archives are rejected until bundletool targeting can safely choose one variant.
- Ordinary installation requires Android confirmation. Silent installation, forced downgrade, and signature-mismatch replacement require a compatible privileged path.
- The signature-mismatch option does not patch Android. It is intended only for rooted devices already using Core Patch or a compatible system modification and Android may still reject the package.
- APK installation and OBB placement are separate operations. The app may install successfully even if Android blocks the OBB destination; WizeFiles reports that partial result and offers retry.
- Secure shred is limited to supported writable local paths. Flash wear levelling, snapshots, backups, and synchronized copies prevent a guarantee of physical erasure.
- TTC files are previewed as collections; WizeFiles does not install fonts.

### Installation notes

- Version 0.7.0 uses the Beta application ID and updates earlier Beta builds in place when signed with the same key.
- Back up important files and use disposable packages, OBB data, and shred targets for initial testing.
- Review package names, version codes, signing certificates, selected splits, and OBB destinations before confirming installation.
- Beta builds expire 30 days after compilation.

### Integrity

- APK: `WizeFiles_v0.7.0_beta.apk`
- SHA-256: `8a6aec81ee01344fa65f060c39298aace0c151e1e67d44ecdf4da8ecfc5fec1b`
- Release: [WizeFiles v0.7.0 Beta](../../releases/tag/v0.7.0)

## Version 0.6.5 — 2026-08-17

### What changed

- Unified Browser and Vault view controls: both support List and Grid layouts, responsive automatic column counts, manual column overrides, consistent selection, and the same floating action menu order.
- Refined adaptive grids for phones, tablets, foldables, and desktop-width windows by capping icon size and increasing useful density on larger displays.
- Fixed stale, clipped, or square-looking recycled icons after changing the grid count, switching icon shapes, or scrolling.
- Updated Vault with a Browser-style view/sort toolbar action, localized folder/file counts, corrected system-bar insets, a single-row Import Files/Lock Vault control, and consistent create dialogs.
- Updated the universal and Vault floating action menus to offer New File, New Folder, New Secure Folder, then Connect Cloud Drive.
- Updated App Manager selection actions: Uninstall is disabled when a system app is included, Enable/Disable reflects the selected apps' state, and the redundant Select all action was removed.
- Matched Browser New File and New Folder dialogs to Vault, including rounded surfaces, balanced field margins, and consistent keyboard/inset handling.
- Added user-controlled local crash reports. WizeFiles does not automatically upload them; the tester chooses whether and how to share sanitized diagnostics.
- Improved text-editor save readiness and unsaved-change tracking, browser list refreshes, location icons, Paste visibility, Settings/system insets, translations, and other visual details.
- Added a branded edge-to-edge navigation drawer header while retaining readable storage and navigation actions.

### Please test

- Switch Browser and Vault repeatedly between List, Auto Grid, and manual grid counts; rotate or resize the window, scroll quickly, change icon shape/theme, and confirm icons remain rounded, correctly sized, and attached to the right item.
- Verify Auto Grid uses sensible density on compact phones, large phones, tablets, foldables, landscape, and desktop-width windows; verify a manual count remains in effect until Auto is selected again.
- Select files and folders in Browser and Vault grid/list layouts and verify highlighting, action availability, back behavior, item counts, view/sort controls, and the floating action menu order.
- In App Manager, select user, system, enabled, disabled, and mixed app sets. Confirm system selections cannot be uninstalled and Enable/Disable is shown only when the selection has an unambiguous applicable state.
- Create files, normal folders, and secure folders from both Browser and Vault; check field margins, rounded dialogs, keyboard insets, validation, cancellation, and persistence.
- Trigger and inspect a local crash report using a non-sensitive test scenario, then confirm nothing is uploaded until the user explicitly shares it.
- Edit text, leave with and without saving, navigate rapidly, and exercise Settings/About/navigation drawer flows across light, dark, dynamic-color, and large-screen configurations.

### Known limitations

See [Known Issues](KNOWN_ISSUES.md#version-065-limitations) for deliberate beta boundaries and current reporting guidance.

### Installation notes

- Version 0.6.5 uses the Beta application ID and updates earlier Beta builds in place when signed with the same key.
- Local crash reports can contain filenames, paths, or device details. Review and sanitize them before sharing publicly.
- App Manager backups contain APK files only; application data, accounts, preferences, and private files are never included.
- Beta builds expire 30 days after compilation.

### Integrity

- APK: `WizeFiles_v0.6.5_beta.apk`
- SHA-256: `b927e4cd89c0b4b3b8e05f0aad8ff43003c332799fae5e6e4647bba41d4b3bf6`
- Release: [WizeFiles v0.6.5 Beta](../../releases/tag/v0.6.5)


## Version 0.6.4 — 2026-08-12

### What changed

- Added App Manager with installed-package inventory, filters, search, package details, app opening, Android-confirmed uninstall, sharing, and provider-aware APK backup. Single-APK apps export as `.apk`; split packages export as checksum-described `.apks`.
- Added focused built-in image and video previews, service-backed background audio playback, a read-only PDF reader, offline EPUB/MOBI-family e-book viewing, and a bounded saved-web-document viewer for HTML/XHTML, MHTML, CHM, and MAFF.
- Added bounded preview support for ICO/CUR, TIFF/BTF, TGA-family, and camera-RAW sources, plus LibVLC fallback for specialist audio/video codecs that Media3 cannot decode.
- Expanded read-only browsing across extensive archive, filesystem, and disk-image families, including RAR/RAR5, CAB, ISO/UDF, WIM, XAR, DMG, APFS, EXT, FAT, HFS/HFS+, NTFS, SquashFS, QCOW2, VDI, VHD/VHDX, VMDK, MBR/GPT, and split archive sets.
- Added secure APK signing and verification for v1, v2, v3, and detached v4 signatures with provider-aware staging, key-store import/generation, Transfer Center recovery, and certificate reporting.
- Added AAB upload-key signing and verification plus APKS, XAPK, and APKM package-container workflows with post-write validation and preservation of non-APK payloads.
- Added the WizeFiles Pro entitlement foundation, signed offline license verification, Google Play Billing integration, app-styled purchase/restore UI, and enforced Free/Pro feature boundaries.
- Beta remains time-limited Pro and never launches real checkout. Production purchase activation remains dependent on backend verification and a signed entitlement.
- Hardened minified startup initialization and reflective component discovery. Missing production backend/public-key configuration now fails safely to Free.

### Please test

- App Manager inventory, filters, selection behavior, regular and split-package backups, sharing, cancellation, remote destinations, package info, and Android-confirmed uninstall.
- Local, SAF, root, Vault, archive, network, and cloud sources in every built-in viewer; include corrupt, oversized, password-protected, disconnected, and unsupported samples.
- Common and specialist audio/video formats, Media3-to-LibVLC fallback, background playback, notification controls, audio focus, Bluetooth, and headset unplug behavior.
- Read-only archive and disk-image browsing, split-volume discovery, guarded extraction, traversal rejection, and expansion limits.
- APK/AAB/APKS/XAPK/APKM signing and verification with imported and generated keys, wrong passwords, output conflicts, interruption recovery, tampering, and detached v4 sidecars.
- About → WizeFiles Pro, active Beta entitlement state, and access to every gated advanced workflow. Confirm Beta never offers or launches Google Play checkout.


### Installation notes

- Version 0.6.4 uses the Beta application ID and updates earlier Beta builds in place when signed with the same key.
- App Manager backups contain APK files only; application data, accounts, preferences, and private files are never included.
- Package-signing passwords and private-key material must never be included in public issue reports.
- Beta builds expire 30 days after compilation.

### Integrity

- APK: `WizeFiles_v0.6.4_beta.apk`
- SHA-256: published beside the APK on the release page
- Release: [WizeFiles v0.6.4 Beta](../../releases/tag/v0.6.4)

## Version 0.6.3 — 2026-08-07

### What changed

- Added 12 adaptive shapes for file and folder content visuals, with **Squircle** as the default. Built-in glyphs use theme-aware container colors, while image/video thumbnails and APK artwork follow the selected shape.
- Added an **Icon shape** picker under Appearance with live previews for Squircle, Rounded square, Flower, Square, Teardrop, Pebble, Vessel, Pentagon, two Hexagon variants, Heptagon, and Octagon.
- Moved selection commands into a rounded bottom action panel with four context-aware primary actions and a **More** menu. Single-item, multi-file, folder, and mixed selections now expose only valid actions.
- Centralized item actions in selection mode, removed per-item three-dot buttons, applied Material selected-item colors, and made Back clear the active selection before navigating away.
- Grouped Transfer Center, Sync & Backup, PC Access & Local Sharing, and Nearby Transfer under a new **Tools** submenu. Browser and selection-menu icons now use the theme primary color while unavailable actions remain visibly disabled.
- Removed the built-in image and video editors. Media thumbnails, properties, **Open with**, and **Edit with** handoff to installed Android apps remain available.
- Fixed normal-tap opening of remote files whose paths use WizeFiles-managed providers. Rclone and other custom remote paths are now resolved through the app's provider registry, addressing [issue #7](../../issues/7).

### Please test

- Change the icon shape repeatedly and verify list/grid rows, image/video thumbnails, APK artwork, Vault entries, Storage Cleaner results, and conflict previews update correctly in light, dark, black, and dynamic-color themes.
- Test the selection panel with one file, one folder, multiple files, and mixed file/folder selections. Verify Rename, Batch rename, Select all, Share suppression for folders, **More**, and Back behavior in single-pane and dual-pane layouts.
- Confirm Back clears selection before folder navigation and correctly restores any pending Paste or picker panel.
- Open the **Tools** submenu and verify every available destination, icon tint, disabled state, and narrow-screen layout.
- Open remote text files with a normal tap and with **Open with** across rclone/cloud, FTP/FTPS, SFTP, SMB, and WebDAV providers where available.
- Open and edit images and videos through installed external apps, save changes back when supported, and confirm thumbnails and media properties still work.

### Known limitations

- Image and video editing requires a compatible external Android app.
- Archive editing remains limited to unencrypted ZIP, 7z, and TAR.XZ files; unsupported, encrypted, split, nested, and signed formats remain read-only.
- Nearby Transfer still requires Google Play services, supports one sender and one receiver per session, and always copies rather than moves source files.
- Beta builds expire 30 days after compilation.

### Installation notes

- Version 0.6.3 updates installed WizeFiles Beta 0.6.0–0.6.2 builds in place when they use the same beta signing key.
- WizeFiles Beta uses a separate application ID from the future stable app, so their app data remains separate.
- If you reported or reproduced remote-file opening issue #7, retest the same file after updating and share the result on the issue.

### Integrity

- APK: `WizeFiles_v0.6.3_beta.apk`
- SHA-256: published beside the APK on the release page
- Release: [WizeFiles v0.6.3 Beta](../../releases/tag/v0.6.3)

## Version 0.6.2 — 2026-08-06

### What changed

- Added transactional editing for unencrypted ZIP, 7z, and TAR.XZ archives. Supported actions include paste, cut/paste, delete, rename, new folder, keyboard actions, and internal drag-and-drop.
- Integrated archive modifications with Transfer Center and added conflict handling, validation, interruption recovery, and safe replacement of the original archive.
- Fixed the blank bottom band introduced by the dual-pane browser wrapper by restoring the original inset-aware layout contract.
- Added an always-visible Paste command to the file-list overflow menu when clipboard content can be pasted.
- Added distinct Transfer Center, Sync & Backup, and Nearby Transfer icons and normalized enabled menu-icon tinting across light and dark themes.
- Redesigned file-operation panels as compact floating pills with navigation-safe spacing, rounded edges, shared FAB-menu coloring, and left-edge animation.
- Expanded and rounded FAB-menu labels so actions such as **Connect Cloud Drive** are shown in full.

### Please test

- In unencrypted ZIP, 7z, and TAR.XZ archives, add files and folders, create empty folders, rename and delete entries, and exercise Replace, Keep both, Skip, and Cancel conflicts.
- Pause, cancel, or interrupt archive reconstruction and confirm that the original archive remains valid and recovery is available through Transfer Center.
- Paste from local, SAF, SD card, USB, cloud, SMB, FTP/FTPS, SFTP, and WebDAV sources into supported archives where available.
- Check single-pane and dual-pane browsing with gesture and three-button navigation; confirm there is no blank band above the operation panel and that Paste remains discoverable.
- Verify operation-panel height, safe-area gap, left-edge animation, menu-icon tinting, and complete FAB labels in light, dark, and dynamic-color themes.

### Known limitations

- Archive editing is limited to unencrypted ZIP, 7z, and TAR.XZ files.
- Encrypted, split, nested, signed, RAR, ISO, CAB, APK, AAB, JAR, DOCX, XLSX, PPTX, EPUB, and unknown archive formats remain read-only.
- Symbolic links cannot be pasted into archives. Archive reconstruction may require substantial temporary space and time for large local or remote archives; the short final commit phase is non-cancellable.
- Nearby Transfer still requires Google Play services, supports one sender and one receiver per session, and always copies rather than moves source files.
- Beta builds expire 30 days after compilation.

### Installation notes

- Version 0.6.2 updates installed WizeFiles Beta 0.6.0 and 0.6.1 builds in place when they use the same beta signing key.
- WizeFiles Beta uses a separate application ID from the future stable app, so their app data remains separate.
- Back up important files and begin archive-editing tests with data you can recover.

### Integrity

- APK: `WizeFiles_v0.6.2_beta.apk`
- SHA-256: published beside the APK on the release page
- Release: [WizeFiles v0.6.2 Beta](../../releases/tag/v0.6.2)

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

- Direct nearby phone-to-phone transfer was not included in 0.6.0; update to 0.6.1 or later to test it.
- Editing archive contents in place was not included in 0.6.0; update to 0.6.2 or later to test it.
- App Manager/APK backup was not included in 0.6.0; it was added after the 0.6.3 release.
- Beta builds expire 30 days after compilation.

### Installation notes

- WizeFiles Beta is a prerelease. Back up important files and test initially with recoverable data.
- The beta application can be installed separately from the future stable app, and each keeps separate app data.

### Integrity

- APK: `WizeFiles_v0.6.0_beta.apk`
- SHA-256: `70817394cb18696ebf0a08f48c508dfe35961a76df605fb326e3a2c000742b78`
- Release: [WizeFiles v0.6.0 Beta](../../releases/tag/v0.6.0)
