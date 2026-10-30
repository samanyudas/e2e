---
"e2e": patch
---

The terminal, Markdown, JUnit, and trace page reporters now look up each serial group member by its test id instead of scanning the group's members for every result. Report output is unchanged. Reporting time grew with the square of a serial group's size: with 2 retries, it now takes about a third less time for a 1000-member group and about two thirds less for a 3000-member group. Groups of 100 members or fewer see no measurable change.
