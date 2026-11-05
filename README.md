<div align="center">

# Konochi

### Your desktop. Your taste.

A personal collection of native Omarchy plugins by [Alec Xu](https://github.com/xvvhang).

[Explore the plugins](#plugins) · [Screenshots](#screenshots) · [Installation](#installation) · [Feedback](#feedback)

</div>

---

Inspired by *konomi* — preference or taste — Konochi brings small, thoughtful
improvements to the desktop you use every day. Keep your workspaces recognizable,
your windows within reach and uncluttered, your music visible, your dev ports and
proxy routing under control, and your next break on time.

## Plugins

| Plugin | What it does | Plugin ID |
| --- | --- | --- |
| [**Konocontrol**](https://github.com/xvvhang/omarchy-konocontrol-plugin) | A native control center collecting built-in bar widgets into Media, Quick Actions, and Controls. | `konochi.konocontrol` |
| [**Konoports**](https://github.com/xvvhang/omarchy-konoports-plugin) | Local dev servers grouped by process and port, with listening addresses, commands, browser links, and confirmed process termination. | `konochi.konoports` |
| [**Konoproxy**](https://github.com/xvvhang/omarchy-konoproxy-plugin) | Native Mihomo proxy controls, subscriptions, profiles, rules, node selection, latency and exit-region checks, and optional bar traffic rates, with explicitly authorized core setup. | `konochi.konoproxy` |
| [**Konousage**](https://github.com/xvvhang/omarchy-konousage-plugin) | Account-separated ChatGPT coding quotas and reset times for OpenCode V2 and Codex. | `konochi.konousage` |
| [**Konobreak**](https://github.com/xvvhang/omarchy-konobreak-plugin) | Work and break intervals with a bar countdown, notifications, pause/resume, and snoozing. | `konochi.konobreak` |
| [**Konobeat**](https://github.com/xvvhang/omarchy-konobeat-plugin) | Now-playing controls, scrolling track information, a playback timeline with supported seeking, and eight real-audio visualization styles. | `konochi.konobeat` |
| [**Konoview**](https://github.com/xvvhang/omarchy-konoview-plugin) | A fullscreen window overview with live previews, keyboard hints, search, and optional double-Super activation. | `konochi.konoview` |
| [**Konocap**](https://github.com/xvvhang/omarchy-konocap-plugin) | Sliding titlebars only on the focused floating window, with theme integration and no manual Hyprland configuration. | `konochi.konocap` |
| [**Konostat**](https://github.com/xvvhang/omarchy-konostat-plugin) | CPU, GPU, memory, storage, network, fan, and temperature monitoring with configurable bar metrics. | `konochi.konostat` |
| [**Konospaces**](https://github.com/xvvhang/omarchy-konospaces-plugin) | Workspace labels with switchable monochrome icons, application names, or full-color icons, plus special-workspace support and live updates. | `konochi.konospaces` |

Each plugin has its own repository, documentation, license, and issue tracker.
This repository is the series showcase, not an installable Omarchy plugin.

## Screenshots

Screenshots are maintained in this showcase's `assets/` directory or as
`preview.png` in each plugin repository. Select an image to view it at full resolution.

| Konocontrol | Konocap |
| --- | --- |
| [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konocontrol-plugin/main/preview.png" alt="Konocontrol with Media, Quick Actions, and native controls" width="360">](https://github.com/xvvhang/omarchy-konocontrol-plugin/blob/main/preview.png) | [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konocap-plugin/main/preview.png" alt="Konocap showing a titlebar only on the focused floating terminal" width="360">](https://github.com/xvvhang/omarchy-konocap-plugin/blob/main/preview.png) |

| Konoports | Konoproxy |
| --- | --- |
| [<img src="assets/konoports.png" alt="Konoports local dev server, port, launch command, and browser and process controls" width="360">](assets/konoports.png) | [<img src="assets/konoproxy.png" alt="Konoproxy cat bar icon and native proxy controls with an anonymized node label" width="360">](assets/konoproxy.png) |

| Konousage | Konobreak |
| --- | --- |
| [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konousage-plugin/main/preview.png" alt="Konousage account tabs and remaining coding quota" width="360">](https://github.com/xvvhang/omarchy-konousage-plugin/blob/main/preview.png) | [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konobreak-plugin/main/preview.png" alt="Konobreak countdown, work and break durations, and session controls" width="360">](https://github.com/xvvhang/omarchy-konobreak-plugin/blob/main/preview.png) |

| Konobeat | Konostat |
| --- | --- |
| [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konobeat-plugin/main/preview.png" alt="Konobeat playback controls and audio visualizer settings" width="360">](https://github.com/xvvhang/omarchy-konobeat-plugin/blob/main/preview.png) | [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konostat-plugin/main/preview.png" alt="Konostat system monitoring panel and bar metric switches" width="360">](https://github.com/xvvhang/omarchy-konostat-plugin/blob/main/preview.png) |

| Konospaces | Konoview |
| --- | --- |
| [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konospaces-plugin/main/preview.png" alt="Konospaces numbered workspaces with per-window application icons" width="360">](https://github.com/xvvhang/omarchy-konospaces-plugin/blob/main/preview.png) | [<img src="https://raw.githubusercontent.com/xvvhang/omarchy-konoview-plugin/main/preview.png" alt="Konoview live window previews with search and keyboard selection hints" width="360">](https://github.com/xvvhang/omarchy-konoview-plugin/blob/main/preview.png) |

## Installation

Requires **Omarchy Quattro**. Review each plugin's README for dependencies,
permissions, setup instructions, and limitations before installing.

Run only the commands for the plugins you want:

```sh
# Native control center
omarchy plugin add https://github.com/xvvhang/omarchy-konocontrol-plugin --enable

# Local dev servers and ports
omarchy plugin add https://github.com/xvvhang/omarchy-konoports-plugin --enable

# Proxy controls, profiles and rules
omarchy plugin add https://github.com/xvvhang/omarchy-konoproxy-plugin --enable

# Agent subscription usage
omarchy plugin add https://github.com/xvvhang/omarchy-konousage-plugin --enable

# Work and break reminders
omarchy plugin add https://github.com/xvvhang/omarchy-konobreak-plugin --enable

# Music controls and visualizers
omarchy plugin add https://github.com/xvvhang/omarchy-konobeat-plugin --enable

# Window overview
omarchy plugin add https://github.com/xvvhang/omarchy-konoview-plugin --enable

# Focus-only floating titlebars
omarchy plugin add https://github.com/xvvhang/omarchy-konocap-plugin --enable

# System monitoring
omarchy plugin add https://github.com/xvvhang/omarchy-konostat-plugin --enable

# Workspace application icons or names
omarchy plugin add https://github.com/xvvhang/omarchy-konospaces-plugin --enable
```

### Before you start

- **Konocontrol** collects existing built-in Omarchy widgets only, excluding Tray.
  Keep collected widgets enabled in `bar.layout`; third-party plugins stay in the
  bar. It depends on native shell internals and may need updates as Omarchy evolves.
- **Konoports** uses Python 3.9+ and Linux `/proc`/pidfds. It scans current-user
  TCP listeners locally, with heuristic dev-server detection. IPv4/IPv6 listeners
  for the same process and port share one entry with all bind addresses shown;
  the bar icon hides when no dev servers are detected. Stopping requires
  confirmation and affects the entire process; no root/system processes are managed.
- **Konoproxy** needs system Python 3.11+. Enabling the plugin alone installs no
  core and captures no traffic. Settings offers explicitly authorized installation
  of a pinned Mihomo core and dedicated service, with optional boot startup and
  narrowly scoped password-free controls. TUN changes routing and DNS; review
  existing VPNs first. Tailscale coexistence requires verified split routing,
  without an exit node or default routes; see the plugin's routing limitations.
  Opening the panel probes nodes through Google and Cloudflare for latency and
  exit-region checks. Optional bar labels show the selected node's region and
  upload/download rates; both default to off. Use **Settings → Uninstall**
  for optional core/service cleanup; removing or disabling only the plugin can
  leave the service and proxying active.
- **Konousage** needs Python 3 and signed-in OpenCode V2 and/or Codex clients.
  It reads the active clients' credentials and contacts ChatGPT's usage endpoint.
  OpenCode's local API command may start its background service; Codex
  OS-keyring-only sign-in is not supported. It does not modify credentials or
  cache tokens. Read its authentication and privacy documentation before enabling it.
- **Konobreak** needs Python 3 and `notify-send` with action support. Installing
  it does not automatically start a work session.
- **Konobeat** needs Python 3, PipeWire's `pw-cat`, and an MPRIS-compatible player.
  It samples the output monitor, not the microphone, and does not save recordings.
  A playback timeline appears when the player provides valid duration and position;
  dragging seeks only when supported. The widget hides when no track metadata is
  available. Disable `omarchy.media` manually if you want to avoid duplicate
  controls and notifications.
- **Konoview** works through shell IPC. Double-Super activation requires the
  optional manual keybinding setup documented in its repository.
- **Konocap** targets Omarchy 4.5 floating workspaces and automatically builds a
  native extension using CMake, a C++23 compiler, pkg-config, and installed
  Hyprland development dependencies; Python 3.9+ and stock
  `omarchy-hyprland-titlebars` are required. No Hyprland config edits are needed;
  disabling restores stock titlebars. Application-drawn titlebars are unaffected.
  Other Hyprland versions may require source updates; see its compatibility notes.
- **Konostat** uses Python 3 and readable system telemetry. Hardware support
  varies; NVIDIA metrics optionally use an already-installed `nvidia-smi`.
- **Konospaces** needs Hyprland's Lua dispatch interface, Quickshell's Hyprland
  integration, `hyprctl`, Python 3, and `xdg-terminal-exec`. Right-click to cycle
  through monochrome icons, application names, and original full-color icons.
  Disable `omarchy.workspaces` manually if you want to replace the stock widget.

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
For Konoproxy, use its in-panel uninstall flow when also removing the managed
core; the generic plugin-removal command does not run core cleanup.
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
