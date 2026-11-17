# Handover

Last updated: 2026-11-17 10:29 (+08:00)
Updated by: Copilot assistant (model not shown)
Session goal was: Add a short controls explanation below the game in `index.html`.

## 1. Project in one paragraph
Pest Patrol is a browser shooting-gallery game set in a Filipino sari-sari store. Players aim with the mouse and left-click to shoo mosquitoes during a 60-second round. Version one is a single-file game that runs directly in a browser.

## 2. Where things are
- Project folder: `pest-patrol`
- Main files: `index.html` contains the game; `notes/` contains project notes.
- GitHub repo: Not documented.
- Live site: Not documented.
- How to run it: Open `index.html` directly in a browser.
- Project notes: Start with `notes/index.md`; read `notes/memory.md` each session.

## 3. Done and verified
Only things a person checked. Say how.
- [x] Controls text in `index.html`: you confirmed the new `<p class="instructions">` line appears under the game.
- [x] Basic play and scoring: you shot mosquitoes for a few seconds and confirmed the game still plays and the score goes up.

## 4. Done but NOT verified yet
Things the AI changed that nobody has tested.
- None reported. A full round was not played.

## 5. Broken or known issues
- No errors or broken behavior reported. The complete 60-second round has not been tested this session.
- The controls are now explained twice under the game: the new `<p class="instructions">` line and the older "MOVE MOUSE to aim | LEFT CLICK to shoo mosquitoes!" line. Decide which one to keep.

## 6. Decisions (and why)
So the next session doesn't undo them.
- Keep the controls explanation as a paragraph below the game; it makes mouse aiming and left-click shooting clear without changing gameplay.
- Keep the game in `index.html` with no libraries or local server; it should run by opening the file directly.
- Keep rounds at 60 seconds, with mouse aiming and left-click shooting.
- No alternatives were tried or rejected in this session.

## 7. Next steps, in order
The first one should be small enough to finish in one go.
1. Play one full 60-second round and check that the final score screen appears.
2. Click PLAY AGAIN and check that the score, timer, and mosquitoes reset.

## 8. Be careful with
- Do not edit files in `raw/`; they are source documents.
- Preserve the single-file game structure in `index.html`.

## 9. Questions for the human
- None.

## 10. Not in this file on purpose
No API keys, passwords, or real personal or client data. Secrets live:
Location not documented.
