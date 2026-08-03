# Security Policy

## Supported builds

Only the latest WizeFiles Beta release is eligible for beta security investigation. Older beta builds may be unsupported and should be updated before testing.

## Report vulnerabilities privately

**Do not disclose security vulnerabilities in a public issue or discussion.**

Use GitHub's **Security → Report a vulnerability** option for this repository when available. If private vulnerability reporting is not yet enabled, use the private support contact published by WizeFiles in the app or on its official website. Do not include exploit details in a public request for contact.

A useful private report includes:

- Affected WizeFiles version/build
- Android version and device model
- Clear reproduction steps
- Security impact
- Whether user interaction or special permissions are required
- A minimal proof of concept, if safe
- Suggested mitigation, if known

## Sensitive information

Do not send real passwords, access tokens, OAuth authorization codes, cloud configuration files, vault contents, recovery keys, signing keys, or personal documents. Use a test account and redact identifiers whenever possible.

## Response process

A report will be reviewed, reproduced where possible, prioritized by impact and exploitability, and addressed before public disclosure when appropriate. Please allow reasonable time for investigation and remediation.

## Scope

Examples of in-scope concerns include unauthorized file access, credential exposure, vault or biometric bypass, insecure remote-provider handling, unsafe update installation, and permission-boundary violations.

General crashes, feature failures, and non-security data-loss bugs belong in the public issue forms after sensitive information has been removed.
