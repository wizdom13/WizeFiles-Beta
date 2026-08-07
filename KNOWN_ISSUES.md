# Known Issues

One confirmed public defect affects the latest WizeFiles Beta release. A fix has been merged for the next beta but is not included in version 0.6.2.

Release-specific testing risks and limitations are documented here and in the relevant [GitHub release](../../releases). Before reporting a problem, check this page and search [open issues](../../issues).

## Confirmed defect in version 0.6.2

### Normal tap can fail for some remote text files

- **Affected:** Version 0.6.2 when opening some files whose paths use WizeFiles-managed remote providers, including rclone-backed connections.
- **Severity:** Medium. The normal-tap open action can fail or crash, but the remote file is not modified.
- **Workaround:** Select the file, use **Open with**, and choose the text editor explicitly.
- **Status:** Fixed in [WizeFiles PR #93](https://github.com/wizdom13/WizeFiles/pull/93). The fix is awaiting the next beta and reporter validation.
- **Tracking:** [Issue #7](../../issues/7).

## Version 0.6.2 limitations

- Transactional archive editing supports only unencrypted ZIP, 7z, and TAR.XZ archives.
- Encrypted, split, nested, signed, RAR, ISO, CAB, APK, AAB, JAR, DOCX, XLSX, PPTX, EPUB, and unknown archive formats are read-only.
- Archive reconstruction can require substantial temporary storage and time for large local or remote archives. The short final commit phase cannot be cancelled.
- Symbolic links cannot be pasted into archives.
- Nearby Transfer requires Google Play services, supports one sender and one receiver per session, and does not interoperate with Android Quick Share.
- Receiving through Nearby Transfer must be started by the user. Sending always copies and never deletes the sender's source files.
- Beta builds expire 30 days after compilation.

## How this list is maintained

An issue is added here when it is confirmed, affects multiple testers, or needs an important workaround. Each entry should include:

- A short description
- Affected versions, devices, or providers
- Severity
- Workaround, if any
- Link to the tracking issue
- Status: investigating, fix in testing, or resolved in a later build
