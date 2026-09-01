# WizeFiles Beta

**WizeFiles** is a powerful all-in-one Android file manager for local storage, SD cards, USB drives, network shares, cloud storage, archives, media, Android apps, backups, secure storage, and more.

**WizeFiles is free and open source under the GNU GPL v3.0 license.** There are no ads, subscriptions, in-app purchases, paid features, or Pro limits.

> [!IMPORTANT]
> The WizeFiles source code is being prepared for public release and will be added to this repository after the remaining modifications are completed. For now, this repository is the official home for public beta builds, release notes, bug reports, and feedback.

> [!WARNING]
> WizeFiles Beta is for testing. Keep a backup of important files and do not use a beta build as the only copy of critical data.

## Download WizeFiles Beta

Download beta builds only from this repository's [Releases](../../releases) page.

> [!NOTE]
> The current release is **[WizeFiles v0.7.0 Beta](../../releases/tag/v0.7.0)** (build 700), published on 30 August 2026.
>
> Beta builds expire 30 days after compilation. Install a newer beta build to continue testing.

For safety, compare the downloaded APK with the SHA-256 checksum included with the release.

## What's new in 0.7.0

- New built-in installer for **APK, APKS, APKM, and XAPK** packages
- Review app version, signing certificate, permissions, features, and components before installation
- Automatically select the correct split APKs for your device
- Install XAPK expansion/OBB files when included
- Optional root-assisted downgrade and advanced installation options
- **Open** the newly installed or updated app directly after installation
- Open Android packages from other apps using **Open with WizeFiles**
- New **Font Viewer** for TTF, OTF, and TTC fonts
- New **Secure Shred** option for supported local files and folders
- Improved Browser and Vault file-list layout
- Improved file and folder icons using Material 3 styling
- **Trash Bin** replaces the previous Recycle Bin naming
- All previous paid/Pro restrictions removed
- WizeFiles is now licensed under **GPL-3.0**

See the [changelog](CHANGELOG.md#version-070--2026-08-30) for more release details.

# Features

## File manager

- Browse internal storage, SD cards, USB drives, and Android storage providers
- Multiple tabs
- Dual-pane browsing on tablets, foldables, and larger screens
- Drag and drop between panes
- Mouse right-click menus and keyboard shortcuts
- Bookmarks and favorite folders
- Fast search and filtering
- Sort files by name, size, date, type, and other options
- Create, copy, move, duplicate, rename, and delete files and folders
- Advanced batch rename
- Keep-both and conflict handling when files already exist
- File and folder shortcuts
- Modern Material 3 interface

## Trash Bin and secure deletion

- Recover deleted files from the **Trash Bin**
- Permanently delete files when needed
- **Secure Shred** for supported writable local files and folders
- Clear separation between recoverable deletion and irreversible shredding

## Transfer Center

- Run file operations in the background
- See active, completed, failed, and canceled jobs
- View progress and transfer history
- Pause, resume, retry, or cancel supported operations
- Handle file conflicts without losing the rest of a transfer
- Continue long-running work without keeping the file browser open

## Cloud and network storage

Connect to files stored outside your phone:

- FTP / FTPS
- SFTP
- SMB / Windows shares / NAS
- WebDAV
- S3-compatible storage
- Many cloud services through built-in **rclone** support
- Android document providers and cloud apps

WizeFiles can browse, copy, move, rename, and manage files across supported local, network, and cloud locations.

## Sync and backup

- Folder synchronization
- Scheduled sync and backup jobs
- Local-to-local, local-to-remote, and remote-to-local workflows
- Saved backup/sync profiles
- Settings backup and restore

## Nearby Transfer

- Send files directly between nearby Android devices
- QR-based pairing
- No need to upload files to the cloud first
- Transfer progress and history through Transfer Center

## Access your phone from a computer

- Built-in web/browser access
- Local network sharing
- FTP-style access where enabled
- Share files from your phone without installing a separate plugin

## Archives and compressed files

- Create and extract archives
- Browse archives without extracting everything first
- Password-protected archives
- Edit supported archive contents
- ZIP
- 7z
- TAR and compressed TAR formats
- Broad read-only support for many additional archive and disk-image formats

## Image and video viewer

- Built-in image viewer
- Built-in video player
- Open local, network, cloud, and SAF-backed media
- Zoom large images
- GIF, SVG, and WebP support
- Rotate images and video
- Swipe between files in the same folder
- Video seeking and playback-speed controls
- Fullscreen playback
- Media thumbnails and metadata
- **Open with another app** at any time

## Audio player

- Built-in audio player
- Background playback
- Notification and lock-screen controls
- Bluetooth/headset controls
- Album artwork and metadata
- Folder-based play queue
- Seeking and queue controls
- Support for additional media formats through LibVLC fallback

## PDF reader

- Built-in PDF viewer
- Zoom
- Search text
- Text selection
- Password-protected PDFs
- Safe links
- Fullscreen reading
- Two-page layouts on larger screens

## E-books, documents, and text

- E-book reader
- Saved web-document viewer
- Text-file viewer and editor
- Open many common text, script, and configuration files
- Edit supported files directly
- Open or edit files with another Android app when preferred

## Font Viewer

Preview fonts directly inside WizeFiles:

- TTF
- OTF
- TTC
- Font name and format information
- Custom sample text
- Multilingual samples
- Adjustable preview size

Fonts can be opened from local storage, removable storage, network shares, cloud storage, or Android storage providers.

## App Manager

- Browse installed apps
- Search, filter, and sort apps
- Open installed apps
- View app/package details
- Uninstall apps using Android confirmation
- Enable or disable apps where Android allows it
- Share installed APKs
- Back up regular APKs
- Back up split apps as APKS
- Send app-backup jobs to Transfer Center

WizeFiles backs up the application packages, not private application data.

## APK and Android package tools

- Inspect APK files
- View package information
- View signing certificates
- Verify Android package signatures
- APK signing tools
- AAB upload-key signing tools
- Inspect APKS, APKM, and XAPK packages
- Extract/preview icons from supported Android package formats

## Android package installer

Install and review:

- **APK**
- **APKS**
- **APKM**
- **XAPK**

Before installing, WizeFiles can show:

- App version changes
- Signing-certificate compatibility
- Added or removed permissions
- App features and components
- Correct split APKs for your device
- XAPK expansion/OBB files

Normal installations use Android's standard confirmation screen. Advanced root users can optionally use additional downgrade or signature-replacement options on compatible modified devices.

**AAB files can be signed but are not directly installable in WizeFiles.**

## Storage Cleanup

A review-first cleanup wizard helps find:

- Duplicate photos and media
- Duplicate files
- Large files
- APK/package files
- Junk files
- Unused apps
- Storage-heavy folders

Nothing is preselected by default. You choose what to remove, can ignore items, and can decide which duplicate copy to keep.

## Storage Analyzer

- Visual disk-usage overview
- Find folders and files taking the most space
- Quickly identify large storage areas before deleting anything

## Vaults and privacy

- Encrypted Vaults
- App password protection
- Biometric unlock
- Automatic relocking options
- Protect access to the file browser
- Standalone file-encryption tools
- Crash reports stay on the device unless you choose to share them
- No advertising
- No purchase tracking or paid entitlement system

## File Properties

View useful details such as:

- File and folder information
- Size and dates
- Checksums
- Image/audio/video metadata
- APK information
- App signing certificate details
- Permissions

## Android, tablet, foldable, and TV support

- Phones
- Tablets
- Foldables
- Adaptive dual-pane layouts
- Mouse support
- Physical keyboard shortcuts
- Android TV / Leanback support
- Light and dark themes
- Black night mode
- Multiple interface languages
- Customizable file-list behavior and appearance

## Root and Shizuku

Root is **optional**. WizeFiles works normally without it.

Advanced users can enable root or supported Shizuku-assisted functions for operations Android normally restricts. Root-related options are shown only where they are useful.

# How WizeFiles compares

The table below compares commonly advertised capabilities of popular Android file managers. Competitor information is based on publicly documented features reviewed on 7 August 2026; WizeFiles information reflects the product through version 0.7.0.

**Legend:** ✓ Included · ◐ Partial, add-on, plugin, or narrower support · — Not publicly documented

| Feature | **WizeFiles** | Solid Explorer | MiXplorer | Files by Google | X-plore | Total Commander | Cx | ASTRO |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Browsing and organization** |  |  |  |  |  |  |  |  |
| Local, SD card, and USB files | **✓** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Multi-tab browsing | **✓** | ◐ | ✓ | — | — | ◐ | — | — |
| Dual-pane browsing | **✓** | ✓ | ✓ | — | ✓ | ✓ | — | — |
| Drag and drop between panes | **✓** | ✓ | ✓ | — | ◐ | ◐ | — | — |
| Indexed instant search | **✓** | ✓ | ◐ | ◐ | ◐ | ◐ | ◐ | ◐ |
| Advanced batch rename | **✓** | ✓ | ✓ | — | ✓ | ✓ | ◐ | ◐ |
| Bookmarks / favorite folders | **✓** | ✓ | ✓ | ◐ | ✓ | ✓ | ✓ | ✓ |
| **Cloud, network, and transfers** |  |  |  |  |  |  |  |  |
| Direct cloud accounts | **✓ Broad via rclone** | ✓ Broad | ✓ Broad | ◐ Drive backup | ✓ Broad | ◐ Plugins | ✓ | ✓ |
| SMB / LAN client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| FTP / FTPS client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| SFTP client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| WebDAV client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| S3-compatible storage | **✓** | — | ◐ Add-on/provider | — | — | — | — | — |
| Persistent Transfer Center | **✓** | ✓ Resumable | ◐ Task queue | — | ◐ | ◐ | ◐ | ◐ |
| Pause, resume, retry, and job history | **✓** | ✓ | ◐ | — | ◐ | ◐ | ◐ | ◐ |
| Folder sync and scheduled backup | **✓** | ◐ Backup | ◐ Tasks | ◐ Drive backup | — | — | — | ◐ Cloud backup |
| Access phone from PC/browser | **✓ Web** | ✓ Web + FTP | ✓ HTTP + FTP | — | ✓ Web | ◐ Wi-Fi plugin | ✓ FTP | — |
| Direct nearby phone-to-phone transfer | **✓ QR-authenticated** | ◐ Web share | ✓ TCP receive | ✓ Quick Share | ✓ Wi-Fi share | ◐ Plugin | — | — |
| **Archives, security, and recovery** |  |  |  |  |  |  |  |  |
| Create and extract archives | **✓** | ✓ | ✓ Extensive | ◐ Basic | ✓ | ✓ | ✓ | ◐ |
| Password-protected archives | **✓** | ✓ | ✓ | — | ◐ | ◐ | ◐ | — |
| Edit archive contents in place | **✓ ZIP/7z/TAR.XZ** | ◐ | ✓ ZIP | — | ✓ ZIP | ✓ ZIP | — | — |
| Encrypted vault / protected folder | **✓** | ✓ AES-256 | ✓ | ✓ Safe Folder | ✓ | — | — | ✓ |
| Biometric unlock / app lock | **✓** | ✓ Vault | ◐ | ◐ Safe Folder | ✓ Vault | — | — | ✓ Vault |
| Trash Bin / recoverable deletion | **✓** | ◐ | ◐ | ✓ | ✓ | — | ✓ | ◐ |
| **Storage intelligence and power tools** |  |  |  |  |  |  |  |  |
| Storage analyzer / cleanup | **✓** | ✓ | ◐ | ✓ | ✓ Disk Map | — | ✓ | ✓ |
| Duplicate-file finder | **✓** | ✓ | — | ✓ | — | — | ✓ | — |
| Visual disk-map treemap | **✓** | ◐ Analyzer | — | — | ✓ | — | ◐ Charts | — |
| Root access | **✓** | ✓ | ✓ | — | ✓ | ✓ | ◐ Shizuku | — |
| Shizuku-assisted access | **✓** | — | — | — | — | — | ✓ | — |
| Checksums, package signing, and certificate details | **✓** | ◐ | ✓ | — | ◐ | ◐ | ◐ Apps | ◐ Apps |
| Installed-app manager / APK backup | **✓ APK + split APKS** | ◐ App collection | ✓ | ◐ App sharing | ✓ | ✓ | ✓ | ✓ |
| Text editor | **✓** | ✓ | ✓ | — | ◐ Viewer | ✓ | ◐ Viewer | ◐ Viewer |
| Image editing | **◐ External app** | — Viewer | — Viewer | — | — Viewer | — | — | — |
| Video editing | **◐ External app** | — Player | — Player | — Player | — Player | — | — Player | — |
| Built-in gallery / full music player | **— Focused viewers/player** | ✓ | ✓ | ✓ | ✓ | ◐ Player | ✓ | ◐ Media views |
| Android TV support | **✓** | ◐ | ◐ | — | ✓ | ◐ | ✓ | — |
| Deep theme and behavior customization | **✓** | ✓ | ✓ Extensive | — Limited | ✓ | ◐ | ◐ | ◐ |
| **Feature coverage rating** | **9.2/10** | 7.6/10 | 7.4/10 | 2.8/10 | 7.0/10 | 4.6/10 | 5.5/10 | 3.3/10 |
| **UI polish** | **9.0/10** | 9.0/10 | 7.5/10 | 9.5/10 | 6.5/10 | 5.5/10 | 8.0/10 | 7.5/10 |
| **UI character** | **Modern** | Modern | Dense / customizable | Modern / simple | Powerful / dated | Utilitarian / dated | Clean / conservative | Friendly / older |

**Comparison note:** Feature coverage uses one point for full support and half a point for partial, plugin-based, or narrower support across the feature rows above. UI polish is an editorial assessment of visual design, consistency, and general usability rather than an objective benchmark. Features can change over time.

# Free and open source

WizeFiles is now completely free to use:

- No Free/Pro split
- No subscriptions
- No in-app purchases
- No advertisements
- No paid limits on connections, vaults, tools, or advanced features
- Every implemented feature is available to every user

WizeFiles is licensed under the **GNU General Public License v3.0 only (GPL-3.0-only)**.

The source code will be added to this repository after the remaining project modifications are completed.

## Report a problem or suggest a feature

Before reporting a problem, check [Known Issues](KNOWN_ISSUES.md).

- [Bug report](../../issues/new?template=bug_report.yml)
- [Storage/provider problem](../../issues/new?template=provider_problem.yml)
- [Feature request](../../issues/new?template=feature_request.yml)
- [Discussions](../../discussions)

Please remove private information from screenshots and logs before posting them publicly.

## Useful links

- [Releases](../../releases)
- [Changelog](CHANGELOG.md)
- [Known Issues](KNOWN_ISSUES.md)
- [Support](SUPPORT.md)
- [Privacy](PRIVACY.md)
- [Security](SECURITY.md)

---

**WizeFiles** — one file manager for local storage, network shares, cloud accounts, archives, media, Android packages, cleanup, backups, secure storage, and more.