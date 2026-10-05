# Contributing to OPX//77

Thanks for helping. This is the organization-wide guide; a repository with its own
`CONTRIBUTING.md` (for example [opx_infinity](https://github.com/opx77-framework/opx_infinity/blob/main/CONTRIBUTING.md))
adds the rules specific to its code, and that file wins where they differ.

The full reviewer rules are on the documentation site:
**[Contributing](https://opx77-framework.github.io/opx77_doc/docs/guides/contributing)**.

## Before you start

- **Bugs and features start as an issue.** Use the forms in the repository
  concerned. For anything larger than a fix, wait for a maintainer to agree on the
  approach before you write it.
- **Questions go to [Discord](https://discord.gg/xpSuYgEYsU)**, not to the tracker.
- **Security problems never go in public.** See [SECURITY.md](SECURITY.md).
- Issues labelled [`good first issue`](https://github.com/search?q=org%3Aopx77-framework+label%3A%22good+first+issue%22+state%3Aopen&type=issues)
  are a good way in.

## Workflow

1. Fork, or branch if you have write access. **Nothing is pushed to `main`
   directly**: `main` is what the test server must be able to run.

   | Branch | For |
   |---|---|
   | `feat/<thing>` | a new capability |
   | `fix/<thing>` | a defect |
   | `audit/<thing>` | a sweep across the codebase |
   | `docs/<thing>` | documentation only |

2. Make the change, with its tests, and run the repository's checks (see its
   `CONTRIBUTING.md` and the pull request template).
3. Open a pull request. Fill in the template: what changed, **why it was wrong
   before**, which checks you ran, and whether it was verified in game.
4. A maintainer reviews and merges. Squash or merge commits are the maintainer's
   call.

## Commit messages

```
<area>: <what is true now, in plain words>

Why it was wrong before. If it failed silently, what a player saw.
```

`<area>` is the module or folder (`inventory`, `doorlock`, `ui`, `core`, `tests`,
`docs`...). A reader six months out needs the argument, not the diff; they can read
the diff.

## House rules, in one screen

- **The server is authoritative.** Anything that arrives from a client is a request
  from a machine the player owns, and is checked again on the server before it is
  believed.
- **The client has an instruction budget.** A coroutine resume that runs too long is
  killed silently. Long work yields; the test suite has a meter for it.
- **Never a name to a stranger.** In roleplay a name is learnt by meeting someone.
  No screen, toast, chat line or payload reveals a character's name to a player who
  has not been given it.
- **English and French**, always together, for every player-facing text.
- **Never guess an Open77 native.** Look it up with the Open77 devkit for the build
  you target, and declare its permission in the manifest in the same change.
- Comments explain **why**, not what.

## Licence

By contributing you agree that your contribution is licensed under the licence of
the repository you contribute to (MIT for the framework and the library).
Everyone taking part follows the [Code of Conduct](CODE_OF_CONDUCT.md).
