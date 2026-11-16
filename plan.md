# Pest Patrol — Development Plan

## Game Overview

- **Game Name:** Pest Patrol
- **Theme:** Shoo cartoon mosquitoes out of a Filipino sari-sari store before closing time.
- **Game Type:** Shooting Gallery
- **View:** Fixed screen, no moving camera
- **Controls:** Mouse to aim, left-click to shoot
- **Round Duration:** 60 seconds
- **Objective:** Earn the highest possible score by clicking mosquitoes. Smaller mosquitoes are worth more points.
- **Platform:** Browser game

## Technical Requirements

- Use only one file: `index.html`.
- HTML, CSS, and JavaScript must all be inside `index.html`.
- Use HTML Canvas for all game graphics.
- Use the Web Audio API only if sound is added in a future version.
- No libraries or frameworks.
- No external downloads, image files, or sound files.
- The game must run by double-clicking `index.html`.
- No server or installation required.
- Each development step must leave the game playable and working.

---

# Step 1 — First Playable: Store Scene and Mosquito Shooting

**Goal:** Create the sari-sari store environment and implement the main shooting mechanic.

### Features

- Draw a colorful cartoon Filipino sari-sari store using HTML Canvas.
- Include shelves, snacks, drinks, a counter, and store decorations.
- Use a cute, colorful cartoon art style.
- Create three mosquito sizes: small, medium, and large.
- Make mosquitoes appear randomly in different positions.
- Make mosquitoes disappear automatically after a short period.
- Allow the player to aim using the mouse.
- Allow the player to shoot by clicking the left mouse button.
- Mosquitoes disappear when successfully clicked.
- Clicking outside a mosquito has no effect.
- Do not include scoring, timers, health, or end screens yet.

### Acceptance Checks

1. Double-click `index.html`. The sari-sari store scene should appear without errors.
2. Wait a few seconds. Mosquitoes should appear in different locations and disappear automatically.
3. Move the mouse and click a mosquito. It should disappear. Clicking an empty area should do nothing.

---

# Step 2 — Full Game: Scoring and 60-Second Challenge

**Goal:** Add scoring, the countdown timer, game-over screen, and restart functionality.

### Features

- Add a visible score counter.
- Award points according to mosquito size:
  - Small mosquito: 30 points
  - Medium mosquito: 20 points
  - Large mosquito: 10 points
- Add a 60-second countdown timer.
- Display the remaining time clearly.
- Stop mosquito spawning and shooting when the timer reaches zero.
- Display a game-over screen when time runs out.
- Show the player's final score.
- Add a Restart button.
- Restart must reset the score to zero.
- Restart must reset the timer to 60 seconds.
- Restart must clear existing mosquitoes and restart gameplay.

### Acceptance Checks

1. Click mosquitoes of different sizes. Small mosquitoes should award more points than large mosquitoes.
2. Watch the countdown. It should start at 60 seconds and decrease until zero.
3. Let the timer reach zero. The game-over screen should display the final score. Click Restart and confirm that the game starts again with 60 seconds and zero points.

---

# Step 3 — Ready to Share: Final Polish

**Goal:** Improve the presentation and make the game ready to share.

### Features

- Set the browser tab title to `Pest Patrol`.
- Add on-screen control instructions:
  - `Move your mouse to aim.`
  - `Left-click to shoo mosquitoes!`
- Add a credits line: `Made with HTML, CSS & JavaScript`.
- Display a friendly message on phone-sized screens:
  - `Best on a computer!`
- Polish the colors, spacing, typography, and overall presentation.
- Ensure all game elements are properly aligned.
- Ensure the game remains playable after all visual improvements.
- Maintain compatibility with double-clicking `index.html`.

### Acceptance Checks

1. Open the game and confirm that the browser tab displays `Pest Patrol`.
2. Confirm that the control instructions and credits are visible.
3. Resize the browser to a phone-sized screen. The message `Best on a computer!` should appear.

---

## Future Improvements (Not Included in Version One)

The following features are intentionally excluded from the initial version:

- Sound effects using the Web Audio API.
- Power-ups and special abilities.
- Multiple levels and difficulty progression.
- Saved high scores using browser storage.

These features may be added in a future version without changing the core game structure.

---

## Final Project Structure

```text
Pest Patrol/
└── index.html
```

## Development Rules

1. Build only one development step at a time.
2. Always provide the complete updated `index.html` file for each step.
3. Do not implement features assigned to later steps prematurely.
4. After every step, provide exact beginner-friendly testing instructions.
5. Do not proceed to the next step until the current step passes its acceptance checks.
6. Keep the code organized, readable, and beginner-friendly.
7. Do not introduce unnecessary dependencies or additional files.