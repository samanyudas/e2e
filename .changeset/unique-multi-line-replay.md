---
"e2e": patch
---

A multi-line `unique()` value now replays from the cache. The screen shows it on one line, so the end check now looks for it on one line too. Before, the replay missed: `REPLAY_STALE (end-mismatch)` with `--strict-cache`, a hand-off to the agent without it. An older runner reads an entry recorded with this fix as `invalid-entry`.
