# Official Mesh

**An agentic platform for surveillance countermeasures.**

Identity rotation, raw-traffic analysis, coordinated radio silence, and a
console that can tell you what's on the air.

→ **[officialmesh.org](https://officialmesh.org)**

## About

LoRa mesh is cheap and off-grid. The radio layer underneath is observable to
anyone with a receiver — emissions, timing, hardware fingerprints —
regardless of the protocol on top.

Official Mesh is a Meshtastic firmware fork, an LLM-aware operator console,
and the terminal and pocket controls that drive them. Wire-compatible with
stock Meshtastic — interoperates with everything, tells nothing it doesn't
have to.

Built for operators who want to stay quiet.

## Components

| Repo | What it is |
|------|------------|
| [`firmware`](https://github.com/official-mesh/firmware) | Privacy-focused Meshtastic firmware fork — anti-localization, anti-fingerprinting, traffic-analysis-resistance modules on ESP32 / nRF52 with SX1262 / LR1110 radios. |
| [`android`](https://github.com/official-mesh/android) | Android client (and Compose Desktop), downstream fork of Meshtastic-Android, with private-port UI (350–365) for the firmware fork. |
| [`python`](https://github.com/official-mesh/python) | Pip-installable CLI client (`officialmesh`) — exposes the firmware's private-port modules from any shell. |
| [`meshbot`](https://github.com/official-mesh/meshbot) | LLM-powered operator bot — multi-radio (Meshtastic / MeshCore / MQTT), Textual TUI, scheduled hooks, packet forensics, RF privacy controls. |
| [`remote`](https://github.com/official-mesh/remote) | Android foreground-service remote for meshbot — outbound TCP (default port 4404, typically over WireGuard); can bridge a USB-OTG or BLE Meshtastic radio. |
| [`dualboot`](https://github.com/official-mesh/dualboot) | Boot selector for ESP32-S3 devices — switch between stock Meshtastic and MeshCore at power-on, no reflash. |
| [`site`](https://github.com/official-mesh/site) | Marketing site at [officialmesh.org](https://officialmesh.org) (Astro on GitHub Pages). |

## Maintainer

The Official Mesh Admin · `<officialmeshadmin@proton.me>`

## License

Per repo. Most components are AGPL-3.0-only; the firmware and Android client
inherit GPL-3.0 from upstream Meshtastic, with novel files dual-licensed
AGPL-3.0. See each repo's `LICENSE` and `NOTICE.md`.

## Naming

The project name is editorial, not corporate. Official Mesh **is not affiliated
with, endorsed by, licensed from, or authorized by Meshtastic LLC, the
MeshCore project, or any of their maintainers**. "Meshtastic" and "MeshCore"
are referenced nominatively, to identify the upstream projects this suite is
compatible with or forked from.
