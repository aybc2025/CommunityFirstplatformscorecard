# Community First platform scorecard

An interactive dashboard of the Community First New West platform goals, promise versus result, with the Council priorities poll.

**Source:** Patrick Johnstone's newsletter "P@J Newsletter - Election Time!" (Oct 14, 2026), section "Running on a record". The scorecard is the campaign's own assessment of its term. Statuses follow the green, yellow and red shading in the newsletter's table.

## Contents

- `index.html` - the standalone dashboard. Plain HTML, CSS and JavaScript with no dependencies. It loads the two JSON files below, has light and dark modes, and works on phones.
- `data/goals.json` - the 60 goals: theme, topic, what was promised, what was done, and status (`green` = completed or major progress, `yellow` = some progress, `red` = fell short).
- `data/poll.json` - the five Council strategic priorities from the community poll chart (residents and businesses, total agree and strongly agree, plus the prior result where the chart shows one).
- `claude-artifact/index.html` - the same page built for a Claude dashboard artifact. It reads its data through that runtime's `dash` API, so it does not run on its own.

## Run it

The page fetches its data files, so it must be served over http rather than opened as a file.

Locally:

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

On GitHub Pages: in the repository, go to Settings, then Pages, set the source to "Deploy from a branch", and choose the `main` branch and the `/ (root)` folder.
