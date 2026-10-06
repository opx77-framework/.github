<h1 align="center">OPX//77</h1>

<p align="center">
  <strong>A serious-roleplay framework for <a href="https://open2077.net">Open77</a>, the multiplayer platform for Cyberpunk 2077.</strong>
</p>

<p align="center">
  <a href="https://opx77-framework.github.io/opx77_doc/"><img alt="Documentation" src="https://img.shields.io/badge/docs-opx77__doc-c5003c"></a>
  <a href="https://discord.gg/xpSuYgEYsU"><img alt="Discord" src="https://img.shields.io/badge/discord-join-5865F2?logo=discord&logoColor=white"></a>
  <img alt="Status: alpha" src="https://img.shields.io/badge/status-alpha-orange">
  <a href="https://github.com/opx77-framework/opx_infinity/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-blue"></a>
</p>

---

OPX//77 gives an Open77 server what a roleplay city needs: characters, money, jobs and
gangs, an inventory, vehicles with keys and garages, dealerships and clothing stores,
door locks, emotes, phone calls, a HUD, chat and a full staff toolset. It ships as
**one Open77 resource** with a single WebUI, written in Lua and Vue, and built around
three rules:

- **The server decides.** Every request from a client is checked again on the server
  before anything moves: money, items, doors, vehicles.
- **The client stays inside its budget.** Open77 kills a client coroutine that runs too
  long; every hot path is measured by the test suite.
- **Never a name to a stranger.** A character's name is learnt in roleplay, never shown
  by the interface.

## Repositories

| Repository | What it is |
|---|---|
| [**opx_infinity**](https://github.com/opx77-framework/opx_infinity) | The framework: one Open77 resource, 35 modules, one Vue WebUI, one test suite. |
| [**opx_lib**](https://github.com/opx77-framework/opx_lib) | The client library `opx_infinity` is built on, usable by any Open77 resource. |
| [**opx77_doc**](https://github.com/opx77-framework/opx77_doc) | The documentation site: install, configure, every module, every export. |

## Links

- **Documentation**: <https://opx77-framework.github.io/opx77_doc/>
- **Install on a server**: [Getting started](https://opx77-framework.github.io/opx77_doc/docs/getting-started/install)
- **Build on top of it**: [For creators](https://opx77-framework.github.io/opx77_doc/docs/creators)
- **Community**: [Discord](https://discord.gg/xpSuYgEYsU)
- **Support the project**: [Tipeee](https://fr.tipeee.com/dop42/)

## Status

**Alpha.** OPX//77 runs on a test server and changes quickly; APIs and features may change
without notice and it is not yet production-ready. Feedback from operators and players is
what moves it forward.

## Contributing

Contributions are welcome: bug reports with journal lines, in-game verification of open
items, translations, documentation and code.

- Read the [contributing guide](https://github.com/opx77-framework/.github/blob/main/CONTRIBUTING.md)
  and the [Code of Conduct](https://github.com/opx77-framework/.github/blob/main/CODE_OF_CONDUCT.md).
- Look for [`good first issue`](https://github.com/search?q=org%3Aopx77-framework+label%3A%22good+first+issue%22+state%3Aopen&type=issues)
  and [`needs-in-game-test`](https://github.com/search?q=org%3Aopx77-framework+label%3Aneeds-in-game-test+state%3Aopen&type=issues)
  issues.
- Report vulnerabilities privately: see the [security policy](https://github.com/opx77-framework/.github/blob/main/SECURITY.md).

---

<p align="center">
  <sub>OPX//77 is MIT licensed. Copyright © 2026 Luís MOUTA.<br>
  An independent community project, not affiliated with or endorsed by CD PROJEKT RED.</sub>
</p>
