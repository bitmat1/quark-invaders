# 🛸 QUARK INVADERS

A polished Space Invaders + Tower Defence hybrid built with HTML5 Canvas. No dependencies — runs in any browser.

## How to Play

Just open `index.html` in your browser!

### Controls

| Key | Action |
|-----|--------|
| `← →` or `A D` | Move ship |
| `SPACE` or `↑` | Shoot |
| `T` | Place turret at current position (costs 500 pts) |
| `1` | Select Basic Turret |
| `2` | Select Rapid Turret |
| `3` | Select Sniper Turret |

### Gameplay Features

- **5 unique alien types** — hand-drawn with Canvas 2D:
  - 🐡 **Blobfish** (50 pts) — sad, droopy, shoots from below
  - 🦀 **Crab-Bot** (100 pts) — mechanical claws, single giant eye
  - 🪼 **Jellycopter** (150 pts) — jellyfish with spinning helicopter blade
  - 😡 **Grumpy Cube** (200 pts) — pixelated rage block with arms
  - 👁 **The Eye of Malevolence** (1000 pts) — BOSS every 5th wave

- **Tower Defence elements**:
  - Place 3 turret types anywhere on screen (spend 500 pts)
  - Turrets auto-aim and fire at nearest alien
  - Turrets can be destroyed by alien fire

- **Shields** — destructible cover regenerated each wave

- **Power-ups** (drop randomly from kills):
  - ⚡ **Rapid Fire** — triple fire rate for 5 seconds
  - 🛡 **Shield** — invincibility for 5 seconds
  - ❤️ **Extra Life**
  - 🔫 **Extra Turret**

- **Kill streak multiplier** — chains of kills give bonus points
- **Progressive difficulty** — aliens speed up, gain HP, shoot faster per wave
- **Persistent high score table** — saved in localStorage (top 10)
- **Screen shake + particle explosions + screen flash** — game feel polish

### Game Design Principles Applied

- Delta-time movement (smooth across all frame rates)
- Screen shake on impacts
- Particle system for explosions and floating score text
- Enemy juice: wobble/bob animations, glow effects, death spin
- Clear visual hierarchy (player glows cyan, enemies distinct colours)
- Escalating difficulty curve per wave
- Audio feedback (visual cues compensate — add Web Audio API if desired)
- Persistent progression via high scores
