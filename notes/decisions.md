# Decisions that should not change without asking

These decisions come from [raw/plan.md](../raw/plan.md) and the current project state. The bug report file in [raw/](../raw/) is empty, so there are no additional decisions recorded there.

- Keep the whole game in one file, [index.html](../index.html), with inline HTML, CSS, and JavaScript.
- Use HTML canvas for all graphics.
- Do not use libraries, external downloads, or a local server.
- The game must open by double-clicking [index.html](../index.html) in a browser.
- Use a fixed 60-second play round.
- Use mouse aiming and left-click shooting.
- Score mosquitoes by size: small = 30, medium = 20, large = 10.
- When time reaches zero, stop spawning and show the final score with a Restart button.
- Restart must reset the score to 0, the timer to 60 seconds, and clear existing mosquitoes.
- Keep the project as a single-file game and avoid extra assets or dependencies.
- Defer future improvements such as sound effects, power-ups, multiple levels, and saved high scores.
