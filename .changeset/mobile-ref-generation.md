---
"@e2e-dev/mobile": patch
---

Mobile actions name the snapshot each node came from (`@e4~s7`), so agent-device refuses a node that a newer snapshot replaced instead of tapping whatever holds its ref now. The action finds the node again, as it does for any stale node. A `dragTo` sends both nodes from the newest snapshot.
