# TeamUkraine — Інструкції для агента / Agent Instructions

---

## 🇺🇦 Українська

### Контекст
Ця тека керує **Team Ukraine** — командою з велоперегонів на Zwift.
Команда бере участь у періодичних гоночних подіях (ZRL, WTRL TTT, FRR, DIRT, спільнотні заїзди тощо) та координується через Discord.
- YouTube: https://www.youtube.com/@teamukraineesports

### Структура теки
```
TeamUkraine/
├── README.md                         # Огляд команди та посилання
├── roster.md                         # Усі гонщики, категорії, доступність
├── events/
│   ├── _template_event.md            # Шаблон для нової події
│   └── YYYY/                         # Тека року
│       ├── season_overview.md        # Підсумок сезону
│       ├── ZRL/                      # Zwift Racing League
│       ├── WTRL_TTT/                 # Team Time Trial
│       ├── FRR/                      # Fondo Race серія
│       ├── DIRT_Racing/              # DIRT Racing серія
│       └── other/                    # Інші події
└── discord/
    └── announcements.md              # Шаблони дописів у Discord
```

### Правила
1. **Нова подія** → скопіювати `events/_template_event.md` у відповідну теку `events/YYYY/SERIES/`
2. **Новий рік** → створити `events/YYYY/` з підтеками, що дзеркалять структуру 2026
3. **Нова серія** → створити `events/YYYY/SERIES_NAME/README.md` з відстеженням серії
4. **Зміни в ростері** → оновити `roster.md` та кількість по категоріях
5. **Після гонки** → зберегти файл результатів у `events/YYYY/SERIES/` ТА оновити `season_overview.md`
6. **Іменування файлів**:
   - **Файли подій**: `YYYY-MM-DD_SERIES_EventName.md`
   - **Файли результатів**: `YYYY-MM-DD_YYYY-MM-DD_SERIES_EventName[_Route].md`
     - Перша дата = початок події, друга дата = кінець (однакові, якщо одноденна)
     - `SERIES` = код серії (FRR, DIRT, ZRL, WTRL_TTT тощо)
     - `EventName` = коротка назва події/туру (WorldTour, S11 тощо)
     - `_Route` = необов'язковий маршрут для результатів одного етапу
     - Приклади:
       - `2026-02-14_2026-02-22_FRR_WorldTour_TeamStandings.md`
       - `2026-03-03_2026-03-31_DIRT_S11_TeamResults.md`
       - `2026-03-05_2026-03-05_WTRL_TTT_359_Waisted8.md`
7. **Дописи у Discord** → використовувати шаблони з `discord/announcements.md`
8. **Двомовний контент** → усі файли містять спершу Українську (🇺🇦), потім English (🇬🇧), розділені `---`. Обидві секції мають бути синхронізовані.

### Коли користувач просить:
- **Додати гонку/подію**: Створити файл з шаблону, заповнити відомі деталі, запитати склад
- **Оновити результати**: Заповнити таблицю результатів, оновити season overview
- **Додати гонщика**: Оновити roster.md з даними гонщика
- **Підготуватися до гонки**: Запропонувати склад на основі категорій та доступності
- **Підсумувати сезон**: Прочитати всі файли подій за рік і зібрати статистику

---

## 🇬🇧 English

### Context
This folder manages **Team Ukraine**, a cycling e-racing team competing on Zwift.
The team participates in periodic race events (ZRL, WTRL TTT, FRR, DIRT, community events, etc.)
and coordinates via Discord.
- YouTube: https://www.youtube.com/@teamukraineesports

### Folder Layout
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
│       ├── DIRT_Racing/              # DIRT Racing series
│       └── other/                    # Misc events
└── discord/
    └── announcements.md              # Discord post templates
```

### Rules
1. **New event** → copy `events/_template_event.md` into the correct `events/YYYY/SERIES/` folder
2. **New year** → create `events/YYYY/` with sub-folders mirroring 2026 structure
3. **New series** → create `events/YYYY/SERIES_NAME/README.md` with series-level tracking
4. **Roster changes** → update `roster.md` and category distribution counts
5. **After a race** → save result file into `events/YYYY/SERIES/` AND update `season_overview.md`
6. **File naming**:
   - **Event files**: `YYYY-MM-DD_SERIES_EventName.md`
   - **Result files**: `YYYY-MM-DD_YYYY-MM-DD_SERIES_EventName[_Route].md`
     - First date = event start, second date = event end (same date if single-day)
     - `SERIES` = series code (FRR, DIRT, ZRL, WTRL_TTT, etc.)
     - `EventName` = short event/tour name (WorldTour, S11, etc.)
     - `_Route` = optional route name for single-stage results
     - Examples:
       - `2026-02-14_2026-02-22_FRR_WorldTour_TeamStandings.md`
       - `2026-03-03_2026-03-31_DIRT_S11_TeamResults.md`
       - `2026-03-05_2026-03-05_WTRL_TTT_359_Waisted8.md`
7. **Discord posts** → use templates from `discord/announcements.md`
8. **Bilingual content** → all files use Ukrainian (🇺🇦) first, then English (🇬🇧), separated by `---`. Keep both sections in sync when editing.

### When User Asks To:
- **Add a race/event**: Create event file from template, fill known details, ask for lineup
- **Update results**: Fill results table in event file, update season overview
- **Add a rider**: Update roster.md with rider details
- **Prepare for a race**: Generate lineup suggestions based on roster categories & availability
- **Summarize season**: Read all event files for the year and compile stats
