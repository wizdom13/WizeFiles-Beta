# WizeFiles Beta

Official public beta channel for **WizeFiles**, a modern Android file manager.

Use this repository to download test builds, report bugs, and share feedback. **The WizeFiles source code is proprietary and is not included in this repository.**

> [!WARNING]
> Beta builds may contain defects, incomplete features, or changes that affect stored settings and app data. Keep backups of important files and do not use a beta build as the only copy of critical data.

## Download a beta build

Download APKs only from this repository's [Releases](../../releases) page. Each release should include:

- The APK and its version/build number
- Release notes and the areas that need testing
- Known limitations or migration warnings
- A SHA-256 checksum for integrity verification

Do not download WizeFiles Beta APKs from mirrors or third-party websites.

## What WizeFiles offers

WizeFiles is designed for local, removable, network, and cloud storage. Depending on the build and Android device, beta testing may cover:

- Local storage, SD cards, USB drives, and Android Storage Access Framework locations
- FTP, SFTP, SMB, WebDAV, S3, and cloud accounts
- Multiple tabs and adaptive dual-pane browsing
- Copy, move, rename, delete, archive, and extraction workflows
- Advanced batch rename and indexed search
- Transfer Center, folder synchronization, and scheduled jobs
- Duplicate detection, storage cleanup, and visual disk analysis
- Encrypted vault, biometric protection, root, and Shizuku features

Features under active development may not be present or complete in every beta release. The release notes are authoritative for each build.

## How WizeFiles compares

The following comparison is based on features publicly documented by each developer and WizeFiles' current product implementation, reviewed on 3 August 2026.

**Legend:** ✓ Included · ◐ Partial, add-on, or narrower support · — Not publicly documented

| Feature | **WizeFiles** | Solid Explorer | MiXplorer | Files by Google | X-plore | Total Commander | Cx | ASTRO |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Browsing and organization** | | | | | | | | |
| Local, SD card, and USB files | **✓** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Multi-tab browsing | **✓** | ◐ | ✓ | — | — | ◐ | — | — |
| Dual-pane browsing | **✓** | ✓ | ✓ | — | ✓ | ✓ | — | — |
| Drag and drop between panes | **—** | ✓ | ✓ | — | ◐ | ◐ | — | — |
| Indexed instant search | **✓** | ✓ | ◐ | ◐ | ◐ | ◐ | ◐ | ◐ |
| Advanced batch rename | **✓** | ✓ | ✓ | — | ✓ | ✓ | ◐ | ◐ |
| Bookmarks / favorite folders | **✓** | ✓ | ✓ | ◐ | ✓ | ✓ | ✓ | ✓ |
| **Cloud, network, and transfers** | | | | | | | | |
| Direct cloud accounts | **✓ Broad via rclone** | ✓ Broad | ✓ Broad | ◐ Drive backup | ✓ Broad | ◐ Plugins | ✓ | ✓ |
| SMB / LAN client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| FTP / FTPS client | **✓ FTP** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| SFTP client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| WebDAV client | **✓** | ✓ | ✓ | — | ✓ | ◐ Plugin | ✓ | — |
| S3-compatible storage | **✓** | — | ◐ Add-on/provider | — | — | — | — | — |
| Persistent Transfer Center | **✓** | ✓ Resumable | ◐ Task queue | — | ◐ | ◐ | ◐ | ◐ |
| Pause, resume, retry, and job history | **✓** | ✓ | ◐ | — | ◐ | ◐ | ◐ | ◐ |
| Folder sync and scheduled backup | **✓** | ◐ Backup | ◐ Tasks | ◐ Drive backup | — | — | — | ◐ Cloud backup |
| Access phone from PC/browser | **— Planned** | ✓ Web + FTP | ✓ HTTP + FTP | — | ✓ Web | ◐ Wi-Fi plugin | ✓ FTP | — |
| Direct nearby phone-to-phone transfer | **—** | ◐ Web share | ✓ TCP receive | ✓ Quick Share | ✓ Wi-Fi share | ◐ Plugin | — | — |
| **Archives, security, and recovery** | | | | | | | | |
| Create and extract archives | **✓** | ✓ | ✓ Extensive | ◐ Basic | ✓ | ✓ | ✓ | ◐ |
| Password-protected archives | **✓** | ✓ | ✓ | — | ◐ | ◐ | ◐ | — |
| Edit archive contents in place | **—** | ◐ | ✓ ZIP | — | ✓ ZIP | ✓ ZIP | — | — |
| Encrypted vault / protected folder | **✓** | ✓ AES-256 | ✓ | ✓ Safe Folder | ✓ | — | — | ✓ |
| Biometric unlock / app lock | **✓** | ✓ Vault | ◐ | ◐ Safe Folder | ✓ Vault | — | — | ✓ Vault |
| Recycle bin / recoverable deletion | **✓** | ◐ | ◐ | ✓ | ✓ | — | ✓ | ◐ |
| **Storage intelligence and power tools** | | | | | | | | |
| Storage analyzer / cleanup | **✓** | ✓ | ◐ | ✓ | ✓ Disk Map | — | ✓ | ✓ |
| Duplicate-file finder | **✓** | ✓ | — | ✓ | — | — | ✓ | — |
| Visual disk-map treemap | **✓** | ◐ Analyzer | — | — | ✓ | — | ◐ Charts | — |
| Root access | **✓** | ✓ | ✓ | — | ✓ | ✓ | ◐ Shizuku | — |
| Shizuku-assisted access | **✓** | — | — | — | — | — | ✓ | — |
| Checksums, APK, and permission details | **✓** | ◐ | ✓ | — | ◐ | ◐ | ◐ Apps | ◐ Apps |
| Installed-app manager / APK backup | **—** | ◐ App collection | ✓ | ◐ App sharing | ✓ | ✓ | ✓ | ✓ |
| Text editor | **✓** | ✓ | ✓ | — | ◐ Viewer | ✓ | ◐ Viewer | ◐ Viewer |
| Image editing | **✓** | — Viewer | — Viewer | — | — Viewer | — | — | — |
| Video editing | **✓** | — Player | — Player | — Player | — Player | — | — Player | — |
| Built-in gallery / full music player | **— Removed** | ✓ | ✓ | ✓ | ✓ | ◐ Player | ✓ | ◐ Media views |
| Android TV support | **✓** | ◐ | ◐ | — | ✓ | ◐ | ✓ | — |
| Deep theme and behavior customization | **✓** | ✓ | ✓ Extensive | — Limited | ✓ | ◐ | ◐ | ◐ |
| **Feature coverage rating** | **8.4/10** | 7.6/10 | 7.4/10 | 2.8/10 | 7.0/10 | 4.6/10 | 5.5/10 | 3.3/10 |
| **UI polish** | **9.0/10** | 9.0/10 | 7.5/10 | 9.5/10 | 6.5/10 | 5.5/10 | 8.0/10 | 7.5/10 |
| **UI character** | **Modern** | Modern | Dense / customizable | Modern / simple | Powerful / dated | Utilitarian / dated | Clean / conservative | Friendly / older |

**Method:** The feature coverage rating gives full support one point and partial, plugin-based, or narrowly scoped support half a point across the feature rows above. UI polish is an editorial assessment of current visual language, consistency, and mainstream usability—not a laboratory measurement. Feature availability is based on publicly documented product information and may change over time.

## Before testing

1. Read [TESTING.md](TESTING.md).
2. Review [KNOWN_ISSUES.md](KNOWN_ISSUES.md) and the release notes.
3. Back up important data.
4. Install or update the APK according to the release instructions.
5. Test only with data you can recover until the build is proven reliable on your device.

Whether a beta can be installed beside the stable app depends on that release's application ID and signing configuration. Check the release notes before installing.

## Report a problem

Choose the form that best fits:

- [Bug report](../../issues/new?template=bug_report.yml) for reproducible app defects
- [Storage/provider problem](../../issues/new?template=provider_problem.yml) for cloud, NAS, SAF, SD card, or USB issues
- [Feature request](../../issues/new?template=feature_request.yml) for focused product suggestions
- [Discussions](../../discussions) for general feedback and testing conversations

Before submitting, search existing issues and remove private information from screenshots and logs.

> [!CAUTION]
> Never publish passwords, access tokens, OAuth codes, rclone configuration files, private filenames, server addresses, account names, personal documents, signing material, or recovery keys.

Security vulnerabilities must not be reported through public issues. Follow [SECURITY.md](SECURITY.md).

## Useful documents

- [Testing guide](TESTING.md)
- [Known issues](KNOWN_ISSUES.md)
- [Changelog](CHANGELOG.md)
- [Support](SUPPORT.md)
- [Privacy information](PRIVACY.md)
- [Security policy](SECURITY.md)
- [Proprietary distribution terms](LICENSE.md)

## Repository scope

This repository contains beta documentation, feedback templates, and release binaries only. It does not accept source-code pull requests and does not grant permission to copy, modify, redistribute, or create derivative works from WizeFiles except where applicable law requires otherwise.

Copyright © WizeFiles. All rights reserved.
