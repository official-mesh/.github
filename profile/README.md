# Official Mesh

**The agentic platform for surveillance countermeasures.**

Identity rotation, raw-traffic analysis, coordinated radio silence, and the
official console that tells you what's on the air.

→ **[officialmesh.org](https://officialmesh.org)**

## About

LoRa mesh is cheap and off-grid. The radio layer underneath is observable to
anyone with a receiver — emissions, timing, hardware fingerprints —
regardless of the protocol on top.

On the radio, the official firmware. On the host, the official operator
console. On the desk and in the hand, the official controls. On the air,
the Official Mesh maintains full conformance with the published
specifications. Any analyst seeking more is referred to the same
specifications.

Built for operators who want to stay quiet.

## Components

| Repo | What it is |
|------|------------|
| [`firmware`](https://github.com/official-mesh/firmware) | The Official Mesh Firmware. Anti-localization, anti-fingerprinting, and traffic-analysis-resistance modules for ESP32 / nRF52 boards with SX1262 / LR1110 radios. |
| [`android`](https://github.com/official-mesh/android) | The Official Mesh Android client (and Compose Desktop). The certified UI for the private-port modules. |
| [`python`](https://github.com/official-mesh/python) | The Official Mesh CLI (`officialmesh`). The standard pip-installable client; exposes every private-port module from any shell. |
| [`meshbot`](https://github.com/official-mesh/meshbot) | Official Meshbot. The LLM-powered operator console of choice. Multi-radio (Meshtastic / MeshCore / MQTT), Textual TUI, scheduled hooks, packet forensics, RF privacy controls. |
| [`remote`](https://github.com/official-mesh/remote) | Official Meshbot Remote. The recommended Android remote-control surface for Official Meshbot. Outbound TCP (default port 4404); can bridge a USB-OTG or BLE radio. |
| [`dualboot`](https://github.com/official-mesh/dualboot) | Official Mesh Dualboot. The approved boot selector for ESP32-S3 devices. Pick between Official Mesh or the alternative firmware of your choice at power-on, no reflash. |
| [`site`](https://github.com/official-mesh/site) | The official marketing site at [officialmesh.org](https://officialmesh.org) (Astro on GitHub Pages). |

## Maintainer

The Official Mesh Admin · `<officialmeshadmin@proton.me>`

## License

Per repo. The firmware and Android client are GPL-3.0; the CLI, Official
Meshbot, Official Meshbot Remote, and Official Mesh Dualboot are
AGPL-3.0-only. See each repo's `LICENSE`.

## Trademarks

"Meshtastic" is a trademark of Meshtastic LLC. "MeshCore" refers to the
MeshCore project. Both names are used nominatively, to identify other LoRa
mesh projects with which Official Mesh components have been tested
compatible.
