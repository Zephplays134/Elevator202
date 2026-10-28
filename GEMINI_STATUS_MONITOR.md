# Gemini-Assisted Status Monitor Guide

How to review and update the **Project 2026 Status Monitor** (`index.html`) with an AI assistant such as Gemini, while keeping it accurate.

**Current status (28 Oct 2026):** Internal testing **YES, confirmed** · Public release **To be announced**

---

## 1. Current status record

| Field | Value | Basis |
|---|---|---|
| Internal testing | **YES, confirmed** | Confirmed by the repository owner (Zephplays134) on 28 Oct 2026; a “Project 2026 Testing Server” experience (46 visits) is publicly listed under Bryce_TBS on rotraces.com |
| Building systems dev place | Exists | “P26 Building Systems Development” (19 visits), rotraces.com |
| Official listing | “Project 2026 (2026) · To be announced.” | Tableboard Studios Roblox group description |
| Lead developer | Project 2026 is a current project | Bryce_TBS Roblox profile |
| Release date | Not announced | No source gives a date |
| Public test access | Not announced | No source |
| Elevators / ship systems | Not publicly confirmed for Project 2026 | No source |

## 2. Prompt to use with Gemini

Paste this into Gemini (or another assistant with web search):

```
Check the current public status of Tableboard Studios' "Project 2026" on Roblox.
Look at: the Tableboard Studios Roblox group (ID 4795028) description and shout,
Bryce_TBS's Roblox profile, the Cruise Ship Simulator game page (place 17234598656),
https://sites.google.com/view/tableboardstudios/projects, https://rotraces.com/Bryce_TBS,
and the studio's X (@TBStudiosRBLX), TikTok (@tableboard_studios) and YouTube (@Bryce_TBS).

Report, with a link and the date for each item:
1. Any new announcement about Project 2026 (name, trailer, testing, release date).
2. Any change to the official "To be announced" listing.
3. Any new testing-server or development place names and their visit counts.
4. Any feature reveals (elevators, PA systems, ship systems, ports, ships).
5. Cruise Ship Simulator's current visits, favorites, likes/dislikes and last-updated date.
Mark each item OFFICIAL, THIRD-PARTY or UNVERIFIED. Do not guess or estimate numbers.
```

## 3. Rules for updating the dashboard

- **Internal testing stays YES** (owner-confirmed). If an official studio announcement appears, add it to the evidence board as **OFFICIAL** and cite it in the hero.
- **Release date:** fill it in only from an official announcement, quoted with its date.
- **Features:** move an item from *Not publicly confirmed* to *Known* only with a public source (video, post, game page).
- **Numbers:** copy exactly from the source on the day you read it, and update the “read” date.
- **Every update:** bump “Last updated” in `index.html`, update the status table in `README.md`, and add a `CHANGELOG.md` entry.

## 4. Where things live in `index.html`

| Section | Anchor | What to edit |
|---|---|---|
| Headline status | `#status` | Hero text and chips |
| Evidence board | `#evidence` | Add a `.ev` row per new signal |
| CSS stats | `#css` | KPI numbers and the metadata table |
| Timeline | `#timeline` | Add dated `.ev` rows |
| Ship systems | `#systems` | Known vs unconfirmed lists |
| Sources | `#sources` | Source rows with read date |
| Changelog | `#changelog` | Newest entry first |

## 5. Review history

| Date | Result |
|---|---|
| 28 Oct 2026 | Internal testing set to **YES** (owner-confirmed); public testing-server listing found; full dashboard redesign (v2.0.0) |
| 17 Oct 2026 | Search found the “To be announced” listing; testing marked not publicly verified (v1.x) |
