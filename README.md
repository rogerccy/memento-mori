# Life Clock

A life countdown app inspired by *Die With Zero* and Stoic memento mori. See exactly how much time you have left — as a grid of every week of your life, a live ticking countdown, and a free-time estimate that accounts for sleep and work.

**Live:** https://rogerccy.github.io/memento-mori/

## Features

- **Live countdown** — years, months, weeks, and days remaining, ticking in real time
- **Life progress bar** — a thin bar showing the exact percentage of your life lived
- **Life-in-weeks grid** — every week rendered as a small box; past weeks filled, current week highlighted in amber, future weeks empty; hover to see age and week number; year labels every 5 years
- **Stats panel** — summers left, weekends left, full moons left, days remaining, hours remaining
- **Free time remaining** — adjustable for sleep hours/day, work hours/day, work days/week, and retire age; shows waking non-work hours left before and after retirement
- **Daily quote** — a rotating Stoic / philosophical quote (Seneca, Marcus Aurelius, Epictetus, and others)
- **EN / 中文** language toggle
- **GitHub Gist sync** — settings sync to a private Gist (`die-with-zero-settings.json`) across devices
- **Local fallback** — works without a GitHub account via `localStorage`

## Inputs

| Field | Default | Notes |
|---|---|---|
| Date of birth | — | Required |
| Expected lifespan | 80 yrs | Adjustable 60–100 |
| Sleep hrs/day | 8 | For free time calculation |
| Work hrs/day | 8 | For free time calculation |
| Work days/week | 5 | For free time calculation |
| Retire age | 65 | Free time increases after this age |

## Setup

1. Open the app and paste a GitHub Personal Access Token with `gist` scope ([create one here](https://github.com/settings/tokens/new?scopes=gist&description=life-clock))
2. Enter your date of birth and adjust lifespan if needed
3. Settings save automatically — any device with the same token restores your data instantly
