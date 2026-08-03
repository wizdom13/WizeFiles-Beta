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
