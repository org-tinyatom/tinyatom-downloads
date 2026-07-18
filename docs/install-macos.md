# Install TinyAtom on macOS

TinyAtom 0.1 requires an Apple silicon Mac running macOS 13 or later.

1. Download the arm64 DMG from the [TinyAtom releases page](https://github.com/org-tinyatom/tinyatom-downloads/releases/latest).
2. Verify the downloaded file against `SHA256SUMS.txt` from the same release:

   ```sh
   shasum -a 256 ~/Downloads/TinyAtom-*.dmg
   ```

3. Open the DMG and drag **TinyAtom** to **Applications**.
4. Eject the DMG, then open TinyAtom from Applications.
5. Confirm macOS identifies the developer and does not report that the application is damaged or unverified.

TinyAtom creates no atom library until the app starts. Runtimes such as FFmpeg and whisper.cpp are not bundled; install them later from Settings only when needed.

If macOS blocks a correctly downloaded release, do not bypass Gatekeeper with `xattr`, disabled security settings, or an unsigned copy. Re-download the current release and report the exact warning through [TinyAtom support](../SUPPORT.md).
