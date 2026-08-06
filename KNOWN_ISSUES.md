# Known Issues

No confirmed public defects are currently listed for the latest WizeFiles Beta release.

Release-specific testing risks and limitations are documented here and in the relevant [GitHub release](../../releases). Before reporting a problem, check this page and search [open issues](../../issues).

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
