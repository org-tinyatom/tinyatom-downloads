# TinyAtom Desktop Privacy

Last updated: July 18, 2026

This document describes the TinyAtom 0.1 desktop application. The website privacy policy is published at [tinyatom.app/privacy](https://tinyatom.app/privacy).

## Local data

TinyAtom stores settings, logs, installed-atom metadata, atom workspaces, atom databases, linked-file permissions, downloaded runtimes, and models on the user's Mac. The default atom library is `~/TinyAtom`; a user can select another library. Electron application data and logs use the standard per-user macOS application locations.

TinyAtom does not currently include product analytics, advertising trackers, an installation identifier, or automatic crash-report upload. **Copy diagnostics** writes a redacted report to the local clipboard. **Open logs** opens a local folder. Neither action uploads data.

## Network requests

The desktop application can make these requests:

- fetch the public atom catalog and its signature;
- check the public TinyAtom release feed for updates;
- download an application update only after the user chooses Download;
- download a selected runtime or speech model after its signed descriptor is enabled and the user chooses Download;
- access a configured public or private company GitHub catalog;
- publish atom source and metadata to GitHub after the user starts a publish action;
- let an installed atom use network access when that capability is declared and granted.

Those requests disclose ordinary network information, including the user's IP address, to the destination service. GitHub, Hugging Face, atom publishers, company catalog operators, and other destinations apply their own privacy terms.

## Coding agents and user-controlled services

TinyAtom can launch third-party coding-agent command-line tools. Prompts, workspace content, account identifiers, and related data handled by an agent are governed by that agent provider's terms and settings. TinyAtom does not operate those services. Users should review the selected provider before sending confidential material.

Atoms can request capabilities such as files, microphone, camera, screen capture, clipboard, location, Bluetooth, notifications, external links, or network access. macOS and TinyAtom permission controls apply where implemented, but users remain responsible for reviewing an atom and its declared access.

## Diagnostics and support

The copied diagnostic report excludes environment variables, tokens, signing paths, user file names, atom document contents, terminal output, and raw release-provider responses. Logs can contain operational error context. Review any log before sharing it, and never post credentials or private atom data in a public support issue.

Support requests and anything a user deliberately attaches are processed by the service receiving that request. TinyAtom does not automatically send the report or logs.

## Deletion

Users can uninstall an atom with or without deleting its runtime data. Removing TinyAtom itself does not silently delete the atom library. See [Uninstall TinyAtom on macOS](docs/uninstall-macos.md) for the separate application, settings, logs, library, and managed-runtime locations.
