# Manual runtime setup

TinyAtom checks managed storage and compatible tools already available on the Mac before offering a managed action. Use **Settings → Dependencies** to inspect each dependency, cancel an active task, recheck the computer, or open its official manual source.

## Automatic installation

Managed executable downloads and archive imports require a signed public artifact descriptor for the current macOS architecture. TinyAtom's public descriptor catalog is not populated yet, so FFmpeg, FFprobe, or whisper.cpp may show `descriptor-unavailable` and keep their managed actions unavailable. This is a public-release blocker until the official artifacts have been published and tested over the real network.

When descriptors are enabled, TinyAtom verifies artifact size, SHA-256, signed receipts, archive structure, architecture, and executable health before publishing a runtime to `<atom-library>/.tinyatom/cache/runtimes`. A failed action remains visible as a typed failure without exposing local paths in copied application diagnostics.

## Manual sources and accepted files

| Dependency | Official manual source | Current path |
| --- | --- | --- |
| FFmpeg and FFprobe | [FFmpeg macOS downloads](https://ffmpeg.org/download.html#build-mac) | Install a compatible system suite, then choose **Recheck**. |
| whisper.cpp CLI | [ggml-org/whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Managed download/import remains unavailable until a signed descriptor is published. |
| Whisper model | [whisper.cpp models](https://huggingface.co/ggerganov/whisper.cpp/tree/main) | Select a compatible `.bin` model through **Import file**. |

Do not copy executables directly into managed storage. A system-installed FFmpeg suite can be used when both FFmpeg and FFprobe pass the version and compatibility probes.

Do not download executable archives from an untrusted mirror and do not disable verification to force an incompatible build.
