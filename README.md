# WizeFiles Beta

Official public beta channel for **WizeFiles**, a modern Android file manager.

Use this repository to download test builds, report bugs, and share feedback. **The WizeFiles source code is proprietary and is not included in this repository.**

> [!WARNING]
> Beta builds may contain defects, incomplete features, or changes that affect stored settings and app data. Keep backups of important files and do not use a beta build as the only copy of critical data.

## Download a beta build

Download APKs only from this repository's [Releases](../../releases) page.

> [!NOTE]
> The current release is **[WizeFiles v0.6.3 Beta](../../releases/tag/v0.6.3)** (Android build 603), published on 7 August 2026. Download `WizeFiles_v0.6.3_beta.apk` and its SHA-256 checksum from that release.
>
> Beta builds expire 30 days after compilation. Install a newer beta build to continue testing.

Each release should include:

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
- Copy, move, rename, delete, archive, extraction, and transactional ZIP/7z/TAR.XZ editing workflows
- Media-aware thumbnails and properties with **Open with** and **Edit with** handoff to installed Android apps
- Adaptive file/folder icon shapes and theme-aware content visuals
- Advanced batch rename and indexed search
- Transfer Center, folder synchronization, and scheduled jobs
- Direct WizeFiles-to-WizeFiles Nearby Transfer with one-time QR verification
- Duplicate detection, storage cleanup, and visual disk analysis
- Encrypted vault, biometric protection, root, and Shizuku features

Features under active development may not be present or complete in every beta release. The release notes are authoritative for each build.

<h2 align="center">How WizeFiles compares</h2>

The following comparison is based on features publicly documented by each developer and WizeFiles' current product implementation, reviewed on 7 August 2026.

**Legend:** ✓ Included · ◐ Partial, add-on, or narrower support · — Not publicly documented

<table>
  <thead>
    <tr>
      <th align="center">Feature</th>
      <th align="center"><strong>Wize<br>Files</strong></th>
      <th align="center">Solid<br>Explorer</th>
      <th align="center">MiXplorer</th>
      <th align="center">Files by<br>Google</th>
      <th align="center">X-plore</th>
      <th align="center">Total<br>Commander</th>
      <th align="center">Cx</th>
      <th align="center">ASTRO</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th colspan="9" align="left" bgcolor="#1f6feb"><font color="#ffffff"><strong>Browsing&nbsp;and&nbsp;organization</strong></font></th>
    </tr>
    <tr>
      <td align="center">Local, SD card, and USB files</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <td align="center">Multi-tab browsing</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Dual-pane browsing</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Drag and drop between panes</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Indexed instant search</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center">Advanced batch rename</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center">Bookmarks / favorite folders</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <th colspan="9" align="left" bgcolor="#1f6feb"><font color="#ffffff"><strong>Cloud,&nbsp;network,&nbsp;and&nbsp;transfers</strong></font></th>
    </tr>
    <tr>
      <td align="center">Direct cloud accounts</td>
      <td align="center"><strong>✓ Broad via rclone</strong></td>
      <td align="center">✓ Broad</td>
      <td align="center">✓ Broad</td>
      <td align="center">◐ Drive backup</td>
      <td align="center">✓ Broad</td>
      <td align="center">◐ Plugins</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <td align="center">SMB / LAN client</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐ Plugin</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">FTP / FTPS client</td>
      <td align="center"><strong>✓ FTP + FTPS</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐ Plugin</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">SFTP client</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐ Plugin</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">WebDAV client</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐ Plugin</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">S3-compatible storage</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">—</td>
      <td align="center">◐ Add-on/provider</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Persistent Transfer Center</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓ Resumable</td>
      <td align="center">◐ Task queue</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center">Pause, resume, retry, and job history</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center">Folder sync and scheduled backup</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐ Backup</td>
      <td align="center">◐ Tasks</td>
      <td align="center">◐ Drive backup</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">◐ Cloud backup</td>
    </tr>
    <tr>
      <td align="center">Access phone from PC/browser</td>
      <td align="center"><strong>✓ Web</strong></td>
      <td align="center">✓ Web + FTP</td>
      <td align="center">✓ HTTP + FTP</td>
      <td align="center">—</td>
      <td align="center">✓ Web</td>
      <td align="center">◐ Wi-Fi plugin</td>
      <td align="center">✓ FTP</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Direct nearby phone-to-phone transfer</td>
      <td align="center"><strong>✓ QR-authenticated</strong></td>
      <td align="center">◐ Web share</td>
      <td align="center">✓ TCP receive</td>
      <td align="center">✓ Quick Share</td>
      <td align="center">✓ Wi-Fi share</td>
      <td align="center">◐ Plugin</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <th colspan="9" align="left" bgcolor="#1f6feb"><font color="#ffffff"><strong>Archives,&nbsp;security,&nbsp;and&nbsp;recovery</strong></font></th>
    </tr>
    <tr>
      <td align="center">Create and extract archives</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓ Extensive</td>
      <td align="center">◐ Basic</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center">Password-protected archives</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Edit archive contents in place</td>
      <td align="center"><strong>✓ ZIP/7z/TAR.XZ</strong></td>
      <td align="center">◐</td>
      <td align="center">✓ ZIP</td>
      <td align="center">—</td>
      <td align="center">✓ ZIP</td>
      <td align="center">✓ ZIP</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Encrypted vault / protected folder</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓ AES-256</td>
      <td align="center">✓</td>
      <td align="center">✓ Safe Folder</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <td align="center">Biometric unlock / app lock</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓ Vault</td>
      <td align="center">◐</td>
      <td align="center">◐ Safe Folder</td>
      <td align="center">✓ Vault</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">✓ Vault</td>
    </tr>
    <tr>
      <td align="center">Recycle bin / recoverable deletion</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <th colspan="9" align="left" bgcolor="#1f6feb"><font color="#ffffff"><strong>Storage&nbsp;intelligence&nbsp;and&nbsp;power&nbsp;tools</strong></font></th>
    </tr>
    <tr>
      <td align="center">Storage analyzer / cleanup</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">✓ Disk Map</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <td align="center">Duplicate-file finder</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Visual disk-map treemap</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐ Analyzer</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">◐ Charts</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Root access</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">◐ Shizuku</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Shizuku-assisted access</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Checksums, APK, and permission details</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐ Apps</td>
      <td align="center">◐ Apps</td>
    </tr>
    <tr>
      <td align="center">Installed-app manager / APK backup</td>
      <td align="center"><strong>— Planned</strong></td>
      <td align="center">◐ App collection</td>
      <td align="center">✓</td>
      <td align="center">◐ App sharing</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
    </tr>
    <tr>
      <td align="center">Text editor</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">—</td>
      <td align="center">◐ Viewer</td>
      <td align="center">✓</td>
      <td align="center">◐ Viewer</td>
      <td align="center">◐ Viewer</td>
    </tr>
    <tr>
      <td align="center">Image editing</td>
      <td align="center"><strong>◐ External app</strong></td>
      <td align="center">— Viewer</td>
      <td align="center">— Viewer</td>
      <td align="center">—</td>
      <td align="center">— Viewer</td>
      <td align="center">—</td>
      <td align="center">—</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Video editing</td>
      <td align="center"><strong>◐ External app</strong></td>
      <td align="center">— Player</td>
      <td align="center">— Player</td>
      <td align="center">— Player</td>
      <td align="center">— Player</td>
      <td align="center">—</td>
      <td align="center">— Player</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Built-in gallery / full music player</td>
      <td align="center"><strong>— Removed</strong></td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">✓</td>
      <td align="center">◐ Player</td>
      <td align="center">✓</td>
      <td align="center">◐ Media views</td>
    </tr>
    <tr>
      <td align="center">Android TV support</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">—</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">✓</td>
      <td align="center">—</td>
    </tr>
    <tr>
      <td align="center">Deep theme and behavior customization</td>
      <td align="center"><strong>✓</strong></td>
      <td align="center">✓</td>
      <td align="center">✓ Extensive</td>
      <td align="center">— Limited</td>
      <td align="center">✓</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
      <td align="center">◐</td>
    </tr>
    <tr>
      <td align="center"><strong>Feature coverage rating</strong></td>
      <td align="center"><strong>9.2/10</strong></td>
      <td align="center">7.6/10</td>
      <td align="center">7.4/10</td>
      <td align="center">2.8/10</td>
      <td align="center">7.0/10</td>
      <td align="center">4.6/10</td>
      <td align="center">5.5/10</td>
      <td align="center">3.3/10</td>
    </tr>
    <tr>
      <td align="center"><strong>UI polish</strong></td>
      <td align="center"><strong>9.0/10</strong></td>
      <td align="center">9.0/10</td>
      <td align="center">7.5/10</td>
      <td align="center">9.5/10</td>
      <td align="center">6.5/10</td>
      <td align="center">5.5/10</td>
      <td align="center">8.0/10</td>
      <td align="center">7.5/10</td>
    </tr>
    <tr>
      <td align="center"><strong>UI character</strong></td>
      <td align="center"><strong>Modern</strong></td>
      <td align="center">Modern</td>
      <td align="center">Dense / customizable</td>
      <td align="center">Modern / simple</td>
      <td align="center">Powerful / dated</td>
      <td align="center">Utilitarian / dated</td>
      <td align="center">Clean / conservative</td>
      <td align="center">Friendly / older</td>
    </tr>
  </tbody>
</table>

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
