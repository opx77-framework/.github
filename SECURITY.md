# Security policy

OPX//77 runs game servers that real communities play on. A vulnerability in it is
usually a way for one player to take money, items, vehicles or staff powers from
everybody else, or to learn something about another player they should not know.
Please report it privately so it can be fixed before it is used.

## Reporting a vulnerability

**Do not open a public issue, pull request or Discord message describing an
exploit.** An exploit in a public tracker is an exploit handed to every server
running the code.

Report it through a **private GitHub security advisory** on the repository
concerned:

| Repository | Report privately |
|---|---|
| `opx_infinity` (the framework) | <https://github.com/opx77-framework/opx_infinity/security/advisories/new> |
| `opx_lib` (the client library) | <https://github.com/opx77-framework/opx_lib/security/advisories/new> |
| `opx77_doc` (the documentation site) | <https://github.com/opx77-framework/opx77_doc/security/advisories/new> |

Not sure which repository? Use `opx_infinity`. If you cannot use GitHub, contact a
maintainer on [Discord](https://discord.gg/xpSuYgEYsU) **by direct message**, say
you have a security report, and wait for a private channel before sending details.

### What to include

- The component, the version (`version` in its `open77.lua`) or commit, and the
  Open77 server and client builds.
- What an attacker can do, and what they need first (a modified client, a staff
  grant, a second account...).
- Steps to reproduce, or the network event and payload involved.
- Your name or handle if you want to be credited.

## What counts

In scope, for example:

- A network event (`opx:net:*`) or page channel that a modified client can use to
  act without the server's own checks: money, items, vehicles, keys, doors, needs,
  appearance, staff actions.
- A way around an ACL grant, staff immunity or the export caller lists
  (`SERVER.EXPORTS.READ` / `WRITERS`).
- A leak of another player's identity to a stranger (the framework's rule is that a
  name is never shown to someone who has not met the character), their money, or
  their position outside what the game already shows.
- A way to make every client fetch or run something the operator did not configure.
- SQL injection or unbounded writes in the storage layer.

Out of scope:

- Behaviour of the Open77 platform itself (report it to the Open77 team).
- Anything that needs the server operator's own access (`acl.jsonc`, the config
  files, the database).
- Denial of service by flooding a server you do not own.

## What happens next

- We acknowledge the report within **7 days**.
- We confirm or dismiss it, and agree a disclosure date with you, usually once a fix
  is merged to `main`.
- The fix is credited to you in the advisory and the release notes unless you
  prefer otherwise.

## Supported versions

OPX//77 is in **alpha**. Only the latest commit on `main` of each repository is
supported; fixes are not backported.
