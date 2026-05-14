# Galaxy Simulation

A 2D N-body gravitational physics simulation where stars orbit, collide, and merge.

## What it does

- **N-body physics**: Every star gravitationally attracts every other star
- **Collisions**: Stars merge when they touch, conserving momentum and mass
- **Clustered initialization**: Stars spawn in multiple clusters with orbital motion
- **Interactive**: Click anywhere to add a new star

## How to run

Open `galaxy.html` in any modern web browser. No build step, no dependencies.

```bash
# Python 3
python -m http.server 8000

# Or just open the file directly
open galaxy.html  # macOS
xdg-open galaxy.html  # Linux
```

Then navigate to http://localhost:8000/galaxy.html

## Controls

- **Reset**: Generate a new galaxy with the current star count
- **Pause/Resume**: Freeze time
- **Add Star**: Spawn a random star near center
- **Stars slider**: Number of stars for next reset (10-500)
- **Speed slider**: Time dilation (0.1x - 5x)
- **Trail slider**: Motion trail persistence (0 = sharp, 1 = long trails)
- **Click canvas**: Add a star at that location

## The Physics

Each frame:
1. Calculate gravitational force between every pair of stars (F = G·m₁·m₂/r²)
2. Apply forces to update velocities
3. Update positions based on velocities
4. Check for collisions (distance < sum of radii)
5. Merge colliding stars (conserve momentum and mass)

Uses 3 substeps per frame for numerical stability.

## What to watch for

- **Orbital dance**: Stars in clusters orbit their collective center of mass
- **Slingshots**: Close encounters can eject stars at high velocity
- **Mergers**: Large stars consume smaller ones, growing in size
- **Chaos**: Three or more stars in close proximity create unpredictable dynamics
- **Stable binaries**: Two similar-mass stars can orbit each other for a long time

## Parameters

- Gravitational constant G = 100 (tuned for visual interest)
- Max speed cap = 500 (prevents numerical instability)
- Star radius = √(mass) × 0.5
- Softening = 100 (prevents singularities at r→0)

Built for the autonomous coding experiment, May 2026.

