# WizeFiles Beta Testing Guide

Thank you for helping test WizeFiles. Good reports describe one problem clearly, make it reproducible, and avoid exposing private data.

## Safety first

- Back up important files before testing copy, move, rename, delete, archive, extraction, synchronization, or vault features.
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

### Local and removable storage

- Internal storage and app-accessible folders
- Storage Access Framework folders
- SD cards and USB drives
- Permission loss after restart or device reboot
- Copy, move, rename, delete, recycle-bin, and conflict handling

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
- Bottom selection actions for one file, one folder, multiple files, and mixed file/folder selections
- Back clearing selection before navigation and restoring pending Paste or picker panels
- Browser **Tools** submenu availability, icon tinting, and disabled states
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

### Appearance and content visuals

- Switch among all 12 icon shapes and confirm **Squircle** is the default.
- Verify shape previews remain clear in light, dark, black, and dynamic-color themes.
- Check built-in file/folder icons, image/video thumbnails, and APK artwork in list and grid layouts.
- Check the same shapes in Vault, Storage Cleaner, and file-operation conflict previews.
- Change the setting while content is visible, then scroll rapidly and confirm recycled rows do not show stale shapes.
- Verify video play badges and other overlays remain clear and are not clipped incorrectly.

### External media handoff

- Use **Open with** and **Edit with** for images and videos with compatible Android apps.
- Confirm writable edits can be saved back when the external app supports the provided URI.
- Verify media thumbnails and image/audio/video properties remain available after editor removal.
- Test the no-compatible-app case and confirm WizeFiles reports it without crashing.

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
