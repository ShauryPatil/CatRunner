# 🐱 Cat Surfers: Vet Chase

An adrenaline-pumping, 3D endless runner built directly in the browser using **Three.js** and **Tone.js**. Surf on an antigravity hoverboard, leap across railway tracks, dodge oncoming subway trains and Animal Control vans, and outrun the relentless **Dr. Snip** and his oversized vaccine syringe!

---

## 🎮 Gameplay Overview

You are an adventurous tabby cat racing down city railway tracks. Behind you, Dr. Snip is hot on your tail. Stumble or crash into hurdles, and he closes in! Collect golden fish bones, unleash catnip zoomies to smash straight through obstacles, boost your speed with rocket thrusters, and magnetize treats toward you.

---

## ✨ Key Features

### 1. 🏙️ Rich 3D Procedural Subway World
- **Subway Passenger Trains**: Realistic multi-car carriages with brushed stainless steel flanks, blue metro stripes, illuminated cabin windows, rooftop air conditioners, and bogies.
- **Animal Control Vans**: Vet ambulances with emergency flashing lightbars, red cross emblems, slanted windshields, and chrome grilles.
- **Dynamic Track Props**: Overhead steel truss gantries with glowing green traffic signals, railway ties, side barriers, and flanking city skyscrapers.

### 2. 💥 Explosive Zoomies & Crash Immunity
- Collect **Catnip Bags** to trigger invulnerable **Zoomies**!
- An iridescent bubble shield envelops the cat.
- Smashing into roadblocks, ambulances, or subway trains triggers:
  - **Dynamic Launch Physics**: Catapults obstacles forward into the sky with multi-axis tumble rotations.
  - **Expanding Shockwaves & Spark Shards**: Radial emerald ground rings and directional neon spark debris.
  - **Screen Shake & Hit-Stop**: A 45ms impact freeze accompanied by quadratic camera trauma.
  - **Comic Smash Popups**: Animated banners awarded for destruction (`OBLITERATED! +250`, `SUBWAY TRAIN LAUNCHED! +500`).

### 3. ⚡ Power-Up Triad
- 🌿 **Catnip Zoomies (8s)**: Complete crash immunity, 1.25× speed boost, and obstacle-smashing score multipliers.
- ⚡ **Turbo Speed (7s)**: Blazing 1.7× supersonic sprint, dynamic camera FOV expansion, and flaming hoverboard rocket thrusters.
- 🧲 **Fish Magnet (8s)**: Orbiting magnetic halo that vacuums up golden fish bones across all three lanes.

### 4. ☀️ Real-Time 50-Second Day/Night Cycle
- Seamless atmospheric transitions through four distinct phases:
  - **Day (0–40%)**: Crisp sky with warm directional sun and soft volumetric clouds.
  - **Sunset (40–50%)**: Deep amber and twilight purple horizon.
  - **Starry Night (50–85%)**: Deep midnight navy sky with 300 twinkling stars and an orbiting moon.
  - **Sunrise (85–100%)**: Rose-gold dawn illuminating the rails.

### 5. 🐟 Fish Bone Respawn System
- Run ended? Spend your hard-earned **Golden Fish Bones** to revive on the spot!
- Reviving pushes Dr. Snip back to a safe trailing distance, clears obstacles ahead for 35 meters, and grants **4 seconds of invulnerability**.
- Dynamic cost scaling (`10` base bones, `+5` per consecutive revive in a single run).

### 6. 📱 Mobile-First Performance & High-Vis Touch Dock
- **Elevated Touch Dock**: Bottom buttons (`◀ Left`, `▶ Right`, `▼ Slide`, `▲ Jump`) placed above system navigation bars with safe-area insets.
- **Instant Touch Gestures**: Low-latency swipe listener triggers movement mid-drag without waiting for finger release.
- **High-FPS Optimizations**:
  - `THREE.InstancedMesh` batches thousands of rail ties and windows into single draw calls.
  - Shadow-pass disabling on mobile WebGL for steady 60 FPS.
  - Zero-garbage-collection asset caching prevents stutter when generating new track chunks.

---

## 🕹️ Controls

| Action | Desktop / Keyboard | Mobile Touch Gestures | Mobile Touch Dock |
| :--- | :--- | :--- | :--- |
| **Move Left** | `A` or `Left Arrow` | Swipe Left | Tap `◀ Left` |
| **Move Right** | `D` or `Right Arrow` | Swipe Right | Tap `▶ Right` |
| **Jump** | `W`, `Up Arrow`, or `Space` | Swipe Up | Tap `▲ Jump` |
| **Slide** | `S` or `Down Arrow` | Swipe Down | Tap `▼ Slide` |
| **Pause / Resume** | Click `⏸` button | Tap `⏸` button | Tap `⏸` button |
| **Mute / Unmute** | Click `🔊` button | Tap `🔊` button | Tap `🔊` button |

---

## 🛠️ Technology Stack

- **Graphics**: [Three.js](https://threejs.org/) (r128) — WebGL rendering, custom procedural meshes, lighting, and particle effects.
- **Audio**: [Tone.js](https://tonejs.github.io/) — Zero-asset, synthesized sound effects for jumping, sliding, item collection, impacts, and jingles.
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) — Clean, responsive HUD, modals, and animations.
- **Typography**: Google Fonts (*Fredoka One* and *Nunito*).
- **Architecture**: 100% self-contained single-file application (`index.html`) with no local build step required.

---

## 🚀 Getting Started

1. Clone or download this repository.
2. Open `index.html` in any modern web browser (Chrome, Edge, Safari, Firefox).
3. Click **"RUN FOR FREEDOM!"** to start the chase!
