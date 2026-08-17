# Known Issues

No confirmed public defects are currently listed for the latest WizeFiles Beta release, version 0.6.5.

Release-specific testing risks and limitations are documented here and in the relevant [GitHub release](../../releases). Before reporting a problem, check this page and search [open issues](../../issues).

## Version 0.6.5 limitations

These are deliberate product boundaries, not confirmed defects.

- Beta builds provide time-limited Pro access and never launch real Google Play purchases. Production purchase and restore flows require the required store and service configuration.
- App Manager backups include APK files only, not application data, accounts, preferences, databases, or private files. Android confirms every permitted uninstall; WizeFiles disables uninstall when the selection includes a system app.
- App Enable/Disable availability depends on Android package policy, device-owner privileges, and the selected apps' common state.
- APK v4 produces a detached `.idsig` and requires v2 or v3. Package-container formats without a standard sidecar mapping do not expose detached v4.
- Transactional archive editing supports only unencrypted ZIP, 7z, and TAR.XZ. Extended archives, filesystems, and disk images are read-only virtual folders.
- Encrypted/DRM-protected Kindle books and AZW4 Print Replica are rejected. E-book, saved-web, PDF, archive, and disk-image viewers are read-only.
- Image and video editing requires a compatible external Android app.
- Nearby Transfer requires Google Play services, supports one sender and one receiver per session, and does not interoperate with Android Quick Share.
- Receiving through Nearby Transfer must be started by the user. Sending always copies and never deletes the sender's source files.
- Auto Grid responds to the available window width and may change after rotation, resizing, or fold-state changes. A manual column count intentionally overrides Auto until Auto is selected again.
- Crash reports stay local until the user explicitly shares them. Reports may contain filenames, paths, and device details and must be reviewed and sanitized before public posting.
- Beta builds expire 30 days after compilation.

## Resolved in version 0.6.3

### Normal tap could fail for some remote text files

- **Affected:** Version 0.6.2 when opening some files whose paths use WizeFiles-managed remote providers, including rclone-backed connections.
- **Severity:** Medium. The normal-tap open action could fail or crash, but the remote file was not modified.
- **Resolution:** Fixed in WizeFiles Beta 0.6.3.
- **Validation:** Reporter confirmation is requested on [issue #7](../../issues/7).

## How this list is maintained

An issue is added here when it is confirmed, affects multiple testers, or needs an important workaround. Each entry should include:

- A short description
- Affected versions, devices, or providers
- Severity
- Workaround, if any
- Link to the tracking issue
- Status: investigating, fix in testing, or resolved in a later build
