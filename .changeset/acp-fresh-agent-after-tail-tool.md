---
"@e2e-dev/acp": patch
---

A step that starts right after a step that timed out now gets a fresh agent when the old agent runs a tool of its own as it stops. Before, the step failed with `MODEL_PROVIDER_FAILED` ("ACP connection closed"), because it reused the session that tool had closed.
