# WizeFiles Beta

Official public beta channel for **WizeFiles**, a modern Android file manager.

Use this repository to download test builds, report bugs, and share feedback. WizeFiles is free and open-source software licensed under **GPL-3.0-only**. Every implemented feature is available without purchases, subscriptions, advertisements, paid entitlements, or feature paywalls.

> [!IMPORTANT]
> This repository currently contains beta binaries, documentation, feedback templates, and release history. The source tree is being prepared and will be published **in this repository** after the remaining project changes are completed. Until that publication, this repository is not yet a complete source distribution.

> [!WARNING]
> Beta builds may contain defects, incomplete features, or changes that affect stored settings and app data. Keep backups of important files and do not use a beta build as the only copy of critical data.

## Download a beta build

Download APKs only from this repository's [Releases](../../releases) page.

> [!NOTE]
> The current release is **[WizeFiles v0.7.0 Beta](../../releases/tag/v0.7.0)** (Android build 700), published on 30 August 2026. Download `WizeFiles_v0.7.0_beta.apk` and its SHA-256 checksum from that release.
>
> Beta builds expire 30 days after compilation. Install a newer beta build to continue testing.

Each release should include:

- The APK and its version/build number
- Release notes and the areas that need testing
- Known limitations or migration warnings
- A SHA-256 checksum for integrity verification

Do not download WizeFiles Beta APKs from mirrors or third-party websites.

## What's new in version 0.7.0

- Added a verified installer for APK, APKS, APKM, and XAPK packages with device-compatible split selection and pre-install version, signer, permission, feature, and component comparison.
- Added validated XAPK OBB placement after APK success, including rollback, partial-completion reporting, retry, and a root fallback where Android storage restrictions require it.
- Added root-gated downgrade and an explicit, separately confirmed signature-mismatch path for devices already using Core Patch or a compatible system modification.
- Added a TTF, OTF, and TTC Font Viewer with metadata, editable specimen text, multilingual samples, and adjustable preview size.
- Added secure shred for supported writable local files and folders, clearly separated from recoverable Trash Bin deletion and documented with flash-storage limitations.
- Polished the installer with a standard back arrow, accessible Material 3 change colors, a compact options icon, readable warnings, and spaced actions.
- Expanded public documentation for installation security, OBB recovery, Font Viewer behavior, secure shred, and current feature coverage.

See the [changelog](CHANGELOG.md#version-070--2026-08-30) for the full testing focus.

## What WizeFiles offers

WizeFiles combines everyday file management with advanced storage, transfer, package, viewing, and security tools. Availability can still depend on Android permissions, device capabilities, root/Shizuku access, and the limitations noted for each beta release.

### Browsing and organization

- Browse local storage, SD cards, USB drives, Storage Access Framework locations, root filesystems, and Shizuku-assisted paths.
- Use multiple tabs and adaptive dual-pane browsing with independent navigation, search, selection, and cross-pane drag-and-drop.
- Work efficiently with mouse context menus, desktop-style keyboard shortcuts, bookmarks, standard folders, launcher shortcuts, configurable sorting, filtering, and view modes.
- Use indexed search, advanced batch rename, customizable filename display, and adaptive list/grid layouts.
- Choose from multiple file and folder icon shapes with theme-aware container colors and shaped media/APK artwork.

### File operations and Transfer Center

- Copy, move, rename, delete, restore, archive, extract, and perform provider-aware batch operations.
- Resolve conflicts with replace, skip, keep-both, and review-first decisions.
- Monitor durable background work through the persistent Transfer Center with queue controls, progress, pause, resume, retry, cancellation, recovery, timestamps, history, and diagnostics.
- Use the recoverable **Trash Bin** for ordinary deletion or the separate **Secure shred** action for eligible writable local files and folders.
- Preserve staged remote/cloud results in the browser while background uploads finish, with clear pending and failure states.

### Network, cloud, sync, and sharing

- Connect directly to FTP/FTPS, SFTP, SMB, WebDAV, S3-compatible storage, and broad cloud-account support through embedded rclone.
- Use the network and cloud integrations as built-in capabilities—no separate plugin or add-on is required.
- Access the phone from a computer browser, run local HTTP/FTP sharing, and transfer directly between nearby devices with QR-authenticated pairing.
- Create folder-sync and backup profiles with update, mirror, two-way, and move modes.
- Schedule manual, interval, daily, or weekly jobs with Wi-Fi, charging, exclusions, safety limits, conflict handling, and version-retention controls.

### Archives, filesystems, and disk images

- Create and extract common archives, including password-protected workflows.
- Add, remove, and rename entries through transactional ZIP, 7z, and TAR.XZ archive mutation.
- Browse many archive, filesystem, disk-image, and split-volume formats read-only, including RAR/RAR5, CAB, ISO/UDF, WIM, XAR, DMG, APFS, EXT, FAT, HFS/HFS+, NTFS, SquashFS, QCOW2, VDI, VHD/VHDX, VMDK, MBR/GPT, and related sets.
- Apply bounded extraction, staging, traversal protection, expansion limits, cancellation, and cleanup.

### Built-in viewers and editing

- Preview images with large-image tiling, EXIF orientation, GIF/SVG/WebP support, rotation, zoom, and sibling swiping.
- Play video with Media3 and a guarded LibVLC fallback for uncommon formats and codecs.
- Play folder audio through a background MediaSession with notification, lock-screen, headset, Bluetooth, metadata, artwork, seek, and queue controls.
- Read PDFs with progressive rendering, zoom, search, selection, password prompts, safe links, fullscreen, and adaptive tablet pages.
- Read EPUB/MOBI-family e-books and bounded saved-web documents such as HTML/XHTML, MHTML, CHM, and MAFF.
- Preview TTF, OTF, variable fonts, and TTC collections with metadata, editable specimen text, multilingual samples, and adjustable text size.
- Edit text files, inspect file properties and permissions, calculate checksums, view certificates, and hand files to Android's **Open with** or **Edit with** flows.
- Decode specialist image families such as ICO/CUR, TIFF/BTF, TGA, and supported camera RAW sources.

### Android app and package tools

- Manage installed applications with search, filters, package details, opening, enable/disable actions, sharing, Android-confirmed uninstall, and safe system-app restrictions.
- Back up single-APK apps as APK and split applications as checksum-described APKS packages without including private application data.
- Inspect, sign, verify, and work with APK, AAB, APKS, APKM, and XAPK containers, including APK v1/v2/v3/v4 signatures and AAB upload-key workflows.
- Install verified APK, APKS, APKM, and XAPK packages with compatible split selection and pre-install comparison of versions, signers, permissions, features, and components.
- Validate and place XAPK OBB expansion files with rollback, retry, root fallback where required, and honest partial-completion reporting.
- Gate forced downgrade and differently signed replacement behind explicit warnings and compatible privileged/Core Patch environments.

### Storage intelligence and security

- Find duplicate files and media, large files, APKs, unused applications, and other review-first cleanup categories.
- Choose which duplicate to keep, ignore findings, exclude system apps where appropriate, and start with destructive cleanup selections disabled.
- Analyze storage through category summaries and a visual disk-map treemap.
- Protect files with standalone encryption, encrypted vaults, app password/biometric controls, relock policies, and secure settings backup/restore.
- Inspect checksums, APK signatures, signing certificates, permissions, media metadata, and technical file details.
- Generate local crash diagnostics only under user control; nothing is uploaded automatically.

### Interface and device support

- Use Material-styled light, dark, black, dynamic-color, translucent, and immersive appearances.
- Work across phones, tablets, foldables, landscape layouts, Android desktop-style input, and Android TV.
- Configure locale, appearance, behavior, security, default folders, storage connections, archive encoding, root strategy, and backup/restore preferences.
- Keep focused viewers and file workflows without turning WizeFiles into a gallery, full music library, or media editor.

Features under active development may not be present or complete in every beta release. Release notes and [Known Issues](KNOWN_ISSUES.md) are authoritative for the exact downloadable build.

## Open features and GPL-3.0

Every implemented WizeFiles feature is available in every build. There are no in-app purchases,
subscriptions, advertisements, paid entitlements, feature tiers, or artificial limits on remote
connections, vaults, batch operations, sync, package signing, root tools, or built-in servers.

Beta expiration is a testing-safety mechanism only; it is not a license or feature restriction.
Install a current beta to continue testing. WizeFiles is licensed under **GPL-3.0-only**, while
third-party components remain under their respective compatible licenses. The public source tree is
being prepared and will be added to this repository after the remaining changes are completed.

<h2 align="center">How WizeFiles compares</h2>

The following comparison is based on features publicly documented by each developer and WizeFiles' current product implementation, competitor references reviewed on 7 August 2026; WizeFiles implementation updated on 30 August 2026.

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
      <td align="center">Trash Bin / recoverable deletion</td>
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
      <td align="center">Checksums, package signing, and certificate details</td>
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
      <td align="center"><strong>✓ APK + split APKS</strong></td>
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
- [GNU GPL-3.0 license](LICENSE.md)

## Repository scope

This repository currently contains beta documentation, feedback templates, release history, and downloadable binaries. The WizeFiles source tree will be added here after the remaining preparation changes are complete. Once published, this repository will also be the public location for source review, modification, redistribution, and contributions under GPL-3.0-only.

Copyright © 2026 Wissam Chehade. Licensed under GPL-3.0-only.
