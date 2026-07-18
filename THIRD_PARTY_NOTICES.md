# Third-Party Notices

TinyAtom includes or depends on third-party software. Copyright notices and license texts shipped by those projects remain in effect.

## Desktop application

| Component                                | Version        | License                                       |
| ---------------------------------------- | -------------- | --------------------------------------------- |
| Electron, including Chromium and Node.js | 43.1.1         | MIT and bundled Chromium third-party licenses |
| React and React DOM                      | 18.3.1         | MIT                                           |
| xterm.js and addon-fit                   | 5.5.0 / 0.10.0 | MIT                                           |
| better-sqlite3                           | 12.11.1        | MIT                                           |
| node-pty                                 | 1.1.0          | MIT                                           |
| electron-updater                         | 6.8.9          | MIT                                           |
| node-tar                                 | 7.5.17         | BlueOak-1.0.0                                 |
| yauzl                                    | 3.4.0          | MIT                                           |
| Lucide React                             | 1.21.0         | ISC                                           |
| IBM Plex Mono via Fontsource             | 5.2.7          | OFL-1.1                                       |

Electron distributions include `LICENSE` and `LICENSES.chromium.html` with the complete Electron, Chromium, and bundled component notices. Package-specific license texts are also retained with installed production packages.

## Optional managed runtimes

TinyAtom does not bundle FFmpeg, FFprobe, whisper.cpp, or Whisper model files in the application. When a signed runtime descriptor is enabled and a user chooses to download it, TinyAtom installs the separately distributed artifact in managed storage.

- FFmpeg and FFprobe are built from pinned FFmpeg source and distributed under [LGPL-2.1-or-later](https://ffmpeg.org/legal.html). The runtime release contains the applicable license and corresponding pinned source archive.
- whisper.cpp is built from pinned source and distributed under its [MIT license](https://github.com/ggml-org/whisper.cpp/blob/v1.9.1/LICENSE). The runtime release contains the license and pinned source archive.
- Whisper model files are downloaded separately from the [whisper.cpp model repository](https://huggingface.co/ggerganov/whisper.cpp/tree/main) and remain subject to the upstream terms shown there.

Third-party coding agents, Git, GitHub CLI, and manually selected system runtimes are not distributed as part of TinyAtom and remain governed by their providers' terms.
