# Updating the dashboard

A quick checklist for refreshing `index.html`.

## 1. Refresh the numbers

These public Roblox endpoints return JSON you can open straight in a browser:

| Data | URL |
|---|---|
| CSS visits, favorites, playing, updated | https://games.roblox.com/v1/games?universeIds=5897329101 |
| CSS likes / dislikes | https://games.roblox.com/v1/games/votes?universeIds=5897329101 |
| Group members + description | https://groups.roblox.com/v1/groups/4795028 |
| Lead dev profile text | https://users.roblox.com/v1/users/127968748 |
| Badges (timeline dates) | https://badges.roblox.com/v1/universes/5897329101/badges?limit=100 |
| Game passes | https://apis.roblox.com/game-passes/v1/universes/5897329101/game-passes?passView=Full&pageSize=50 |
| Testing-server listing | https://rotraces.com/Bryce_TBS |

Like ratio = up ÷ (up + down) × 100.

## 2. Edit `index.html`

- Hero and status cards: `#status`
- KPI tiles and table: `#css`
- New signals: add an `.ev` row in `#evidence` with a source-type tag
- New dated events: `#timeline`
- Sources table read dates: `#sources`
- Bump **“Last updated”** in the header and footer, and the date in the small script at the bottom (it drives the “x days ago” label).

## 2b. Update the Spencer fire tracker (`spencer-fire/index.html`)

- Check for new reporting on the Shurfine Food Mart fire cause (Tioga County Fire Investigation Team), demolition and any rebuild.
- If an official cause is announced, quote it with attribution and a date in `#answer` and `#officials`, and change the headline only as far as the source says.
- Add dated events to `#timeline`, update `#status`, and add the article to `#sources`.
- Bump “Last updated” in the header and footer.
- Styles live in `spencer-fire/styles.css`. Keep the back link (`../`) at the top so it returns to the main dashboard.

## 3. Keep the repo in sync

- Update the status table and snapshot in `README.md`.
- Add an entry to `CHANGELOG.md` (newest first).
- Add the sources to `docs/SOURCES.md` with the read date.
