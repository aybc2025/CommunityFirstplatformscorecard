# Community First platform scorecard

An interactive dashboard of the Community First New West platform goals, promise versus result, with the Council priorities poll.

**Source:** Patrick Johnstone's newsletter "P@J Newsletter - Election Time!" (Oct 14, 2026), section "Running on a record". The scorecard is the campaign's own assessment of its term. Statuses follow the green, yellow and red shading in the newsletter's table.

## Contents

- `data/goals.json` - the 60 goals: theme, topic, what was promised, what was done, and status (`green` = completed or major progress, `yellow` = some progress, `red` = fell short).
- `data/poll.json` - the five Council strategic priorities from the community poll chart (residents and businesses, total agree and strongly agree, plus the prior result where the chart shows one).
- `dashboard/index.html` - the dashboard page (filters, topic chart, sortable table, poll chart). It was built for a Claude dashboard artifact and reads its data through that runtime's `dash` API, so it does not run as a standalone web page.
