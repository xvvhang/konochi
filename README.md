<div align="center">

# Konochi

### Your desktop. Your taste.

A personal collection of native Omarchy plugins by [Alec Xu](https://github.com/xvvhang).

[Explore the plugins](#plugins) · [Installation](#installation) · [Feedback](#feedback)

</div>

---

Inspired by *konomi* — preference or taste — Konochi brings small, thoughtful
improvements to the desktop you use every day. Keep your workspaces recognizable,
your windows within reach, your music visible, and your next break on time.

## Plugins

| Plugin | What it does | Plugin ID |
| --- | --- | --- |
| [**Konousage**](https://github.com/xvvhang/omarchy-konousage-plugin) | Account-separated ChatGPT coding quotas and reset times for OpenCode and Codex. | `konochi.konousage` |
| [**Konobreak**](https://github.com/xvvhang/omarchy-konobreak-plugin) | Work and break intervals with a bar countdown, notifications, pause/resume, and snoozing. | `konochi.konobreak` |
| [**Konobeat**](https://github.com/xvvhang/omarchy-konobeat-plugin) | Now-playing controls, scrolling track information, and eight real-audio visualization styles. | `konochi.konobeat` |
| [**Konoview**](https://github.com/xvvhang/omarchy-konoview-plugin) | A fullscreen window overview with live previews, keyboard hints, search, and optional double-Super activation. | `konochi.konoview` |
| [**Konostate**](https://github.com/xvvhang/omarchy-konostate-plugin) | CPU, GPU, memory, storage, network, fan, and temperature monitoring with configurable bar metrics. | `konochi.konostate` |
| [**Konospaces**](https://github.com/xvvhang/omarchy-konospaces-plugin) | Workspace labels with per-window application icons, special-workspace support, and live updates. | `konochi.konospaces` |

Each plugin has its own repository, documentation, license, and issue tracker.
This repository is the series showcase, not an installable Omarchy plugin.

## Installation

Requires **Omarchy Quattro**. Review each plugin's README for dependencies,
permissions, setup instructions, and limitations before installing.

Run only the commands for the plugins you want:

```sh
# Agent subscription usage
omarchy plugin add https://github.com/xvvhang/omarchy-konousage-plugin --enable

# Work and break reminders
omarchy plugin add https://github.com/xvvhang/omarchy-konobreak-plugin --enable

# Music controls and visualizers
omarchy plugin add https://github.com/xvvhang/omarchy-konobeat-plugin --enable

# Window overview
omarchy plugin add https://github.com/xvvhang/omarchy-konoview-plugin --enable

# System monitoring
omarchy plugin add https://github.com/xvvhang/omarchy-konostate-plugin --enable

# Workspace application icons
omarchy plugin add https://github.com/xvvhang/omarchy-konospaces-plugin --enable
```

### Before you start

- **Konousage** reads the active clients' credentials and contacts ChatGPT's
  usage endpoint. It does not modify credentials or cache tokens. Read its
  authentication and privacy documentation before enabling it.
- **Konobreak** needs Python 3 and `notify-send` with action support. Installing
  it does not automatically start a work session.
- **Konobeat** needs Python 3, PipeWire's `pw-cat`, and an MPRIS-compatible player.
  It samples the output monitor, not the microphone, and does not save recordings.
  It is hidden when no track metadata is available. Disable `omarchy.media`
  manually if you want to avoid duplicate controls and notifications.
- **Konoview** works through shell IPC. Double-Super activation requires the
  optional manual keybinding setup documented in its repository.
- **Konostate** uses Python 3 and readable system telemetry. Hardware support
  varies; NVIDIA metrics optionally use an already-installed `nvidia-smi`.
- **Konospaces** uses Hyprland's Lua dispatch interface. Disable
  `omarchy.workspaces` manually if you want to replace the stock widget.

Plugins run unsandboxed with your user permissions. Installing from GitHub does
not constitute a security review or imply marketplace approval.

## Manage a plugin

For example, to update, disable, or remove Konobeat:

```sh
omarchy plugin update konochi.konobeat
omarchy plugin disable konochi.konobeat
omarchy plugin remove konochi.konobeat
```

Use the corresponding ID from the table for other plugins. Read the individual
removal instructions to restore stock widgets or remove optional keybindings.
Back up unpushed development changes before removing a plugin: removal can delete
its local Git checkout.

## Feedback

- **Plugin bugs and feature requests:** open an issue in the relevant plugin
  repository linked above.
- **Series ideas and showcase improvements:** [open an issue here](https://github.com/xvvhang/konochi/issues).

## License and credits

This showcase is [MIT licensed](LICENSE). See each plugin repository for its own
license and upstream attribution.

Built for [Omarchy](https://omarchy.org/) and [Quickshell](https://quickshell.org/).
Konochi is an independent community project, not an official Omarchy product.
