# WizeFiles Beta

Official public beta channel and future public source repository for **WizeFiles**, a powerful Android file manager for local, removable, network, cloud, encrypted, and application-package workflows.

**WizeFiles is now free and open-source software licensed under the GNU General Public License v3.0 (GPL-3.0-only).** Every implemented feature is available without advertisements, subscriptions, in-app purchases, paid entitlements, feature tiers, or paywalls.

> [!IMPORTANT]
> WizeFiles is transitioning from the former private development repository to this public repository. The source tree is being prepared for publication and will be added here after the remaining cleanup and modifications are completed. Until then, this repository continues to host public beta builds, release notes, issue tracking, and project documentation.

> [!WARNING]
> Beta builds may contain defects, incomplete changes, or migrations that affect settings and app data. Keep backups of important files and never use a beta build as the only copy of critical data.

## Download a beta build

Download WizeFiles Beta only from this repository's [Releases](../../releases) page.

> [!NOTE]
> The current release is **[WizeFiles v0.7.0 Beta](../../releases/tag/v0.7.0)** (Android build 700), published on 30 August 2026. Download `WizeFiles_v0.7.0_beta.apk` together with its published SHA-256 checksum.
>
> Beta builds expire 30 days after compilation. Install a newer beta build to continue testing.

Each beta release should include:

- The APK and its version/build number
- Release notes and testing focus
- Known limitations or migration warnings
- A SHA-256 checksum for integrity verification

Do not download WizeFiles Beta APKs from mirrors or unofficial third-party websites.

## What's new in version 0.7.0

- Added a verified installer for APK, APKS, APKM, and XAPK packages.
- Added device-compatible split selection and pre-install comparison of versions, signing identities, permissions, features, and components.
- Added validated XAPK OBB placement with rollback, partial-completion reporting, retry, and root fallback where Android storage restrictions require it.
- Added root-gated downgrade support and a separately confirmed signature-mismatch path for devices already using Core Patch or a compatible system modification.
- Added an **Open** action after successful installation when the installed application is launchable.
- Added Android **Open with** routing for APK, APKS, APKM, and XAPK packages.
- Added a TTF, OTF, and TTC Font Viewer with metadata, editable specimen text, multilingual samples, and adjustable preview size.
- Added secure shred for supported writable local files and folders, clearly separated from recoverable Trash Bin deletion.
- Refreshed Browser and Vault list presentation, including Material 3 icon containers, folder item counts, file sizes, and modified dates.
- Renamed the internal Recycle Bin implementation to **Trash Bin**, including migration of existing stored items.
- Removed the former purchase, Pro, entitlement, and license-verification system.
- Licensed WizeFiles under GPL-3.0-only and made every implemented feature available to every user.

See the [changelog](CHANGELOG.md#version-070--2026-08-30) for release-specific testing details.

# Features

WizeFiles is designed as a complete file-management environment rather than only a local file browser. Feature availability can depend on the Android version, storage provider, granted permissions, device capabilities, or optional root/Shizuku access.

## File browsing and organization

- Local internal storage browsing
- SD card and removable-storage support
- USB storage support
- Android Storage Access Framework (SAF) locations and document trees
- Multiple tabs
- Adaptive dual-pane browsing on suitable screens
- Cross-pane drag and drop
- Mouse context menus
- Desktop-style keyboard shortcuts where supported
- Bookmarks and favorite folders
- Standard Android folders and configurable storage roots
- Configurable default directory
- File and folder sorting
- Filtering and search
- Indexed search workflows
- File and folder creation
- Rename and advanced batch rename
- Copy, move, duplicate, and delete operations
- Conflict-aware replacement and keep-both behavior
- File and folder shortcuts
- Android launcher/download entry points
- Configurable filename ellipsizing and list animation
- Adaptive file/folder icon shapes and Material 3 presentation

## Trash Bin and secure deletion

- Recoverable **Trash Bin** deletion for supported local storage
- Restore deleted files from Trash Bin
- Permanent deletion
- Secure shred for supported writable local files and folders
- One-pass zero overwrite, sync, and deletion for eligible local files
- Clear separation between recoverable deletion and irreversible shredding
- Provider-aware restrictions so unsupported SAF, cloud, network, archive, and other remote paths are not falsely presented as securely overwritable

## File operations and Transfer Center

- Background copy, move, delete, archive, extract, and related file jobs
- Persistent Transfer Center
- Progress tracking
- Pause/resume where supported by the operation/provider
- Retry and recovery flows
- Completed, failed, and canceled history
- Start/end timestamps
- Conflict and user-decision handling
- Provider-aware error classification
- Partial-completion reporting
- Metadata-preservation reporting
- Cooperative cancellation
- Resumable/checkpoint-aware workflows where supported
- Queue and durable operation state across long-running transfers

## Local, network, and cloud storage

- Local Android filesystem access
- Root-capable local access where explicitly enabled
- Shizuku-assisted workflows where supported
- SAF/document-provider storage
- FTP and FTPS
- SFTP
- SMB/LAN shares
- WebDAV
- S3-compatible storage
- Direct cloud accounts through embedded rclone
- Generated rclone provider setup
- Simple WebDAV/S3 configuration flows
- rclone configuration import
- Optional rclone power-user setup
- Cloud-app mediated storage entries
- Remote-aware copy, move, delete, traversal, and metadata handling
- Cached/pending transfer presentation for cloud operations

## Synchronization, backup, and scheduled work

- Folder synchronization
- Scheduled sync/backup workflows
- Local-to-remote and remote-aware traversal
- Background execution through Android scheduling infrastructure
- Transfer-state persistence and recovery
- Settings backup and restore
- Tolerant settings restore that can skip obsolete incompatible non-security settings while restoring the remaining configuration
- Backup profile management

## Nearby and device-to-device transfer

- Direct nearby phone-to-phone transfer
- QR-authenticated pairing
- Google Nearby transport integration
- Durable transfer/session state
- Duplicate and late-payload protection
- Payload correlation and recovery rules
- Reconnect-aware behavior after process recreation

## PC/browser and local sharing

- Access-phone-from-PC/browser workflows
- Local web/HTTP sharing features
- Local FTP/server-style sharing features where enabled
- Built-in sharing rather than requiring an external plugin
- Android Share/Open integration
- Save shared content into WizeFiles

## Archives, compressed files, filesystems, and disk images

- Archive browsing
- Archive creation
- Extraction
- Password-protected archive flows
- Transactional mutation for supported writable archive formats
- ZIP workflows
- 7z workflows
- TAR/XZ and related compressed formats
- Broad read-only archive support
- Read-only browsing support for additional filesystem/disk-image formats where supported by the bundled native/archive stack
- Archive filename-encoding options
- Defensive validation for malformed entries, traversal attempts, oversized input, and hostile archive metadata

## Images and video

- Built-in image preview
- Built-in video preview
- Local, SAF, network, and cloud-backed media opening
- Large-image tiled zoom
- EXIF orientation handling
- GIF playback
- SVG rendering
- WebP support
- Rotation
- Sibling-file swiping
- Video play/pause and seeking
- Buffering feedback
- Fullscreen playback
- Playback-speed control
- Media3-based playback
- LibVLC fallback for specialist containers/codecs
- Image, audio, and video thumbnail generation
- Media metadata in File Properties
- **Open with another app** when preferred

## Audio player

- Dedicated service-backed audio playback
- Folder-based playback queue
- Background playback
- Media notification controls
- Lock-screen controls
- Headset/Bluetooth controls
- Metadata and artwork
- Seeking and queue controls
- LibVLC fallback for specialist audio formats while retaining the same media session

## PDF reader

- Built-in read-only PDF viewer
- Progressive page display
- Zoom
- Text search
- Selection
- Password prompts
- Safe hyperlink handling
- Fullscreen mode
- Adaptive two-page tablet layouts

## E-books, documents, and text

- Built-in e-book/document reading workflows
- Saved web-document viewing
- Text viewing and editing
- Broad `text/*` and common script/configuration MIME handling
- Android external edit integration
- Save As support for shared content
- Provider-aware write permission checks before editing

## Font Viewer

- TTF preview
- OTF preview
- TTC preview
- Local, removable, network, cloud, and SAF-backed font opening
- Font format/name metadata
- Editable specimen text
- Multilingual samples
- Adjustable 12–84 sp preview size
- Bounded private staging for provider-backed fonts

## App Manager

- Installed-app inventory for the current Android profile
- Search, filter, and sort installed apps
- Open installed apps
- Inspect application/package details
- Android-confirmed uninstall
- System-app-aware action restrictions
- Enable/disable controls where Android privileges allow them
- Secure APK sharing
- Single APK backup
- Split APK/APKS backup
- Durable app-backup jobs through Transfer Center
- Backups intentionally exclude application data

## APK, package-container, and signing tools

- APK inspection
- APK signing and signature verification workflows
- APK v1/v2/v3/v4 signature-related tooling where applicable
- Certificate details
- AAB upload-key signing workflows
- APKS, APKM, and XAPK container inspection
- Icon extraction/preview workflows for Android package formats
- Split-set validation
- Signing-identity comparison
- Package metadata inspection

## Android package installer

WizeFiles includes its own verified Android package review and installation flow for:

- APK
- APKS
- APKM
- XAPK

Installer capabilities include:

- Safe staging of incoming provider-backed packages
- Device-compatible ABI, density, and locale split selection
- Base/feature split retention
- Package/version consistency checks
- Signer consistency checks across splits
- Comparison against an already installed package
- Version-change presentation
- Permission comparison
- Feature comparison
- Component comparison
- Android PackageInstaller confirmation for ordinary installs
- Root-backed installation when explicitly selected and available
- Explicit root-gated downgrade approval
- Separately confirmed signature-mismatch replacement for devices already using Core Patch or another compatible system modification
- XAPK OBB validation and placement
- OBB rollback and retry after partial completion
- **Open** after successful installation when the target package exposes a launchable activity

**AAB installation is not currently supported.** WizeFiles will not pretend to install AAB files until a proper bundletool-based build pipeline is implemented.

## Storage Cleanup Wizard

- Review-first cleanup workflow
- Duplicate media detection
- Duplicate file detection
- Large-file analysis
- APK/package cleanup categories
- Junk analysis with conservative classification
- Unused-app analysis that excludes system applications
- Clear item details including path/name, size, and date information
- Default all-deselected safety behavior
- Ignore/exclude options
- Ability to choose which duplicate copy to keep
- Provider-aware deletion behavior
- Visual disk/storage analysis

## Encryption, Vaults, and privacy

- Encrypted Vaults
- Vault lifecycle and session management
- Vault lock/relock behavior
- Biometric protection
- App password support
- Optional protection of browser access
- Standalone file-encryption workflows
- Recovery/state protections around vault mutations
- Local crash-report capture controlled by the user
- Crash reports are not automatically uploaded
- Users choose whether to share or delete pending crash reports
- No advertisements
- No analytics-based advertising profile
- No subscription or purchase entitlement system

## File Properties and technical details

- General file/folder properties
- Checksums
- Media metadata
- APK/package information
- Signing certificate details
- Permission information
- Provider/storage metadata
- Native/JNI-assisted low-level file operations where appropriate

## Android integration and device support

- Android 11+ (`minSdk 30` in the current codebase)
- Modern Android storage APIs
- All-files access for full file-manager behavior where granted
- Android Open/Edit/Share integrations
- Android package install/uninstall confirmation flows
- Notifications for long-running operations
- Foreground services for applicable transfers/media playback
- Android TV / Leanback launcher support
- Tablet layouts
- Foldable/adaptive layouts
- Dual-pane behavior on suitable displays
- Mouse and physical-keyboard usability
- Material themes
- Light/dark appearance support
- Black night-mode option
- Configurable locale/language support

## Root and advanced access

Root is optional and is never required for ordinary WizeFiles usage. Where explicitly enabled, advanced workflows can use root for operations Android normally restricts, including selected file operations, package-installation cases, and XAPK OBB placement.

WizeFiles does **not** itself disable Android package verification. The optional signature-mismatch installer path is intended only for devices where the user has already installed Core Patch or another compatible system modification, and Android may still reject the operation.

# Free and open source

WizeFiles has moved away from its former commercial entitlement model.

- No Free/Pro feature split
- No Google Play Billing integration
- No subscriptions
- No in-app purchases
- No signed entitlement/license server
- No feature cardinality limits tied to payment
- No advertisements
- All implemented capabilities are available to all users

WizeFiles is licensed under **GNU GPL-3.0-only**.

The public source tree is currently being prepared and will be added to this repository after the remaining code cleanup and project modifications are completed. Once published, this repository will contain the source, build instructions, license material, development documentation, and contribution workflow alongside beta releases.

## Contributing and feedback

Until the source tree is published, the best way to contribute is to:

- Test the latest beta release
- Report reproducible bugs
- Include Android/device/version information
- Include screenshots or logs when they help explain a problem
- Suggest usability improvements and missing workflows

After the source is published, code contributions and pull requests will also be documented here.

## Known issues

See [KNOWN_ISSUES.md](KNOWN_ISSUES.md) before reporting a problem. Features under active development can vary between beta releases, so the release notes and Known Issues file remain authoritative for a particular build.

## License

WizeFiles is licensed under the **GNU General Public License v3.0 only (GPL-3.0-only)**.

The complete license text and third-party notices will be distributed with the public source tree. Third-party components remain subject to their respective licenses and notices.

---

**WizeFiles** — one file manager for local storage, networks, cloud accounts, archives, media, Android packages, cleanup, synchronization, secure storage, and advanced Android workflows.
