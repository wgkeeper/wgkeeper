<p align="center">
  <img alt="wgkeeper" src="brand/wgkeeper.svg" height="64">
</p>

<p align="center">
  Open-source system for managing WireGuard® infrastructure at scale.
</p>

<p align="center">
  <a href="https://wgkeeper.github.io">Documentation</a> ·
  <a href="https://github.com/wgkeeper/wgkeeper-node">Node</a> ·
  <a href="https://github.com/wgkeeper/wgkeeper-console">Console</a>
</p>

---

wgkeeper consists of a central **Console** for orchestration and **Node** agents that run on each WireGuard server. Together they let you manage peers, allocate IPs, rotate keys, and monitor stats across your entire fleet — without manual `wg` commands.

## Components

| Component | Description | Status |
|-----------|-------------|--------|
| **[Node](https://github.com/wgkeeper/wgkeeper-node)** | Agent on each WireGuard host. REST API for peer management. Go. | [![Release](https://img.shields.io/github/v/release/wgkeeper/wgkeeper-node)](https://github.com/wgkeeper/wgkeeper-node/releases/latest) |
| **[Console](https://github.com/wgkeeper/wgkeeper-console)** | Central admin panel for multi-node management. | [![Release](https://img.shields.io/github/v/release/wgkeeper/wgkeeper-console)](https://github.com/wgkeeper/wgkeeper-console/releases/latest) |

## Getting started

See the **[documentation](https://wgkeeper.github.io/docs)** for installation, configuration, and API reference.

## License

[AGPL-3.0](LICENSE)

WireGuard® is a registered trademark of Jason A. Donenfeld.
