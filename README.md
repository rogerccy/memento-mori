# Die With Zero

A life countdown web app inspired by Bill Perkins' *Die With Zero*. See exactly how much time you have left — not as an abstract number, but as a grid of every week of your life.

**Live:** https://rogerccy.github.io/memento-mori/

## Features

- **Live countdown** — years, months, weeks, and days remaining, ticking in real time
- **Life progress bar** — a thin bar at the top showing the exact percentage of your life lived
- **Life-in-weeks grid** — every week of your life rendered as a small box; past weeks are filled, the current week is highlighted in amber, future weeks are empty outlines
- **Year labels** — the grid labels every 5th year so you can navigate your life at a glance
- **Stats panel** — summers left, weekends left, full moons left, days remaining, hours remaining
- **GitHub Gist sync** — settings (birthdate + expected lifespan) are saved to a private GitHub Gist and sync across any device where you enter the same token
- **Local fallback** — works without a GitHub account; settings are stored in `localStorage`

## Setup

1. Open the app and paste a GitHub Personal Access Token with `gist` scope ([create one here](https://github.com/settings/tokens/new?scopes=gist&description=die-with-zero))
2. Enter your date of birth and expected lifespan (default 80 years, adjustable 60–100)
3. Your settings are saved automatically — return visits load instantly

On a new device, enter the same token and the app finds your existing Gist by filename (`die-with-zero-settings.json`) and restores your settings.
