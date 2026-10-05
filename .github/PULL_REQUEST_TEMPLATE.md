<!--
Branch: feat/<thing>, fix/<thing> or audit/<thing>. Never push to main.
Read CONTRIBUTING.md in the repository first.
-->

## Summary

<!-- What changes, in a few bullets. -->

## Why

<!-- What was wrong before, or what could not be done. If it failed silently, describe what a player saw. Link the issue: "Closes #123". -->

## Checks run

<!-- Tick what you ran; say why if something does not apply. -->

- [ ] `lua tests/run.lua` is green (opx_infinity: with `OPX_LIB_PATH` pointing at an opx_lib checkout)
- [ ] `luac -p` on every changed Lua file
- [ ] `npm run typecheck && npm run build`, and `web/index.html` committed (only if `ui/` changed)
- [ ] `OPX_BUDGET_METER=5000 lua tests/run.lua` lists no new client call site (client changes)
- [ ] English **and** French locale keys added together
- [ ] Docs updated, or a docs issue or PR opened in `opx77_doc`

## Verified in game?

- [ ] Yes. Server build: `...`, client build: `...`. What was tried:
- [ ] No. What still needs an in-game check (add the `needs-in-game-test` label):

## Screenshots

<!-- For anything a player sees. Delete if not applicable. -->
