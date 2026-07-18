# TinyAtom Security Policy

## Supported versions

Security fixes are provided for the latest public TinyAtom release. Pre-release and older builds may be replaced rather than patched.

## Report a vulnerability

Use [GitHub private vulnerability reporting](https://github.com/org-tinyatom/tinyatom-downloads/security/advisories/new) for a suspected vulnerability. Sign in to GitHub, include the affected TinyAtom version, macOS version, reproduction steps, and impact, and attach only the minimum safe evidence.

Do not publish exploit details, credentials, private keys, tokens, personal data, atom contents, or unredacted logs in a public issue. For a non-sensitive product problem, use [TinyAtom support](https://github.com/org-tinyatom/tinyatom-downloads/issues).

TinyAtom will assess a report, reproduce it when possible, and coordinate a fix and disclosure. No fixed response or remediation time is promised for this initial public release.

## Release trust

Public macOS builds must be Developer ID signed, notarized by Apple, and stapled. Release checks verify the app bundle, nested Mach-O signatures, Team ID, hardened runtime, DMG and ZIP copies, update metadata, and published hashes. Atoms use a separate TinyAtom signature and capability-consent system; Apple notarization of TinyAtom does not certify an atom.
