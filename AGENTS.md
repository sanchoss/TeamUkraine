# TeamUkraine — Agent Instructions

## Context
This folder manages **Team Ukraine**, a cycling e-racing team competing on Zwift.
The team participates in periodic race events (ZRL, WTRL TTT, FRR, community events, etc.)
and coordinates via Discord.
- YouTube: https://www.youtube.com/@teamukraineesports

## Folder Layout
```
TeamUkraine/
├── README.md                         # Team overview & links
├── roster.md                         # All riders, categories, availability
├── events/
│   ├── _template_event.md            # Copy for each new event
│   └── YYYY/                         # Year folder
│       ├── season_overview.md        # Year summary
│       ├── ZRL/                      # Zwift Racing League
│       ├── WTRL_TTT/                 # Team Time Trial
│       ├── FRR/                      # Fondo Race series
│       └── other/                    # Misc events
├── results/
│   └── YYYY/                         # Race results, screenshots
└── discord/
    └── announcements.md              # Discord post templates
```

## Rules
1. **New event** → copy `events/_template_event.md` into the correct `events/YYYY/SERIES/` folder
2. **New year** → create `events/YYYY/` with sub-folders mirroring 2026 structure + `results/YYYY/`
3. **New series** → create `events/YYYY/SERIES_NAME/README.md` with series-level tracking
4. **Roster changes** → update `roster.md` and category distribution counts
5. **After a race** → fill in results in the event file AND update `season_overview.md`
6. **File naming**: `YYYY-MM-DD_SERIES_EventName.md` for individual event files
7. **Discord posts** → use templates from `discord/announcements.md`
8. **Bilingual content** → all files use Ukrainian (🇺🇦) first, then English (🇬🇧), separated by `---`. Keep both sections in sync when editing.

## When User Asks To:
- **Add a race/event**: Create event file from template, fill known details, ask for lineup
- **Update results**: Fill results table in event file, update season overview
- **Add a rider**: Update roster.md with rider details
- **Prepare for a race**: Generate lineup suggestions based on roster categories & availability
- **Summarize season**: Read all event files for the year and compile stats
