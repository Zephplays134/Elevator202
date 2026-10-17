# Gemini-assisted Project 2026 status monitor

This is a companion specification for the Elevator202 / Project 2026 public-status dashboard.

## Evidence-based status as of 2026-10-17

- **Project listed publicly:** Yes, based on the public project listing referenced by the existing dashboard.
- **Internal testing:** **Not publicly confirmed.** Do not change this to “Yes” unless a dated official Tableboard Studios/developer source explicitly confirms internal testing. Do not treat a test-server name, rumors, or unrelated repository activity as proof.
- **Release date:** No verified public date in the dashboard.
- **Elevators and ship systems:** Unconfirmed unless an official developer announcement specifies them.

“Not publicly confirmed” is not a claim that private testing is not happening.

## Prompt for Google Gemini

Copy this prompt into Gemini when reviewing new public information:

> Investigate the current public status of Tableboard Studios' Project 2026, related to Roblox Cruise Ship Simulator. Use only public sources and prioritize official Tableboard Studios pages, official Roblox group/game pages, and dated developer announcements. Report:
>
> 1. Is Project 2026 publicly listed? Answer Yes/No/Unclear and cite the source.
> 2. Has internal testing explicitly been confirmed by an official developer source? Answer Yes/No public confirmation found/Unclear. Never infer private testing from a test-server name or rumor.
> 3. What are the newest dated announcements and what changed?
> 4. Has an official release date or launch window been announced?
> 5. Which elevators, ship systems, PA systems, or other features are explicitly confirmed, and which are only speculation?
>
> For every claim, include the source URL, publication/update date if available, and a short explanation of what the source actually proves. If no official confirmation is found, say “Not publicly confirmed,” not “definitely not happening.” Do not invent updates or imply access to private servers, private Discords, or internal builds. End with the date checked.

## Public sources

- [Tableboard Studios Roblox group](https://www.roblox.com/communities/4795028/Tableboard-Studios#!/about)
- [Cruise Ship Simulator on Roblox](https://www.roblox.com/games/17234598656/Cruise-Ship-Simulator)
- [Tableboard Studios projects page](https://sites.google.com/view/tableboardstudios/projects)
- [Secondary group listing](https://www.rolimons.com/group/4795028)

## Important implementation note

This companion prompt does not connect to Gemini or automatically query it. For an actual Gemini API integration, call Gemini from a server-side endpoint and keep the API key in a server secret/environment variable. Never put a private API key in browser JavaScript or commit it to GitHub. Any automated tracker should store source URLs and timestamps and distinguish “no evidence found” from “confirmed no.”
