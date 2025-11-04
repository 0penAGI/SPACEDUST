
# SPACEDUST - Cosmic Strategy & Space Shooter  
**TRY [GAME](http://0penagi.github.io/SPACEDUST)**
**USE $XDUST IN [TELEGRAM](http://t.me/@ARCHITECTUREAIbot)**
![SPACEDUST](https://img.shields.io/badge/SPACEDUST-Cosmic%20Strategy%20%26%20Shooter-00ffff?style=for-the-badge&logo=starship)  
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)  
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)  
![Telegram Web App](https://img.shields.io/badge/Telegram%20WebApp-2CA5E0?style=flat&logo=telegram&logoColor=white)  
![Mobile](https://img.shields.io/badge/Mobile-Optimized-00ff00?style=flat&logo=smartphone)  

## About the Game  
**SPACEDUST** is a hybrid **cosmic strategy + arcade space shooter** built with pure **HTML5, CSS3, and JavaScript**, designed as a **Telegram Web App**.  
Players alternate between **intense 2D combat** in the shooter mode and **strategic galaxy conquest** on a dynamic map, managing resources, upgrading their fleet, and earning **$XSDC** — an in-game token tied to rare cosmic events.  

> **"Defend the Galaxy. Mine the Dust. Conquer the Stars."**  

---

## Features  

| Category | Feature |
|--------|--------|
| **Core Gameplay** | Dual-mode: **Space Shooter** + **Galactic Strategy Map** |
| **Combat** | Power-ups, overheat system, **time dilation**, combo effects |
| **Enemies** | Normal, Code-Drone, Tank, Splitter, **Cosmic Alien Boss** |
| **Strategy** | Sector control, resource mining, mission system |
| **Economy** | Energy, Metals, Crystals, **$XSDC** (crypto-inspired token) |
| **Progression** | Permanent **upgrades** (Fire Rate, Damage, Hull) |
| **Events** | Cosmic Mystery, $XDUST-9001, Hhaas Event |
| **Visuals** | Neon gradients, particle bursts, glitch effects, **Orbitron UI** |
| **Audio** | SFX + dual music tracks (shooter & galaxy) |
| **Persistence** | `localStorage` saves resources, upgrades, $XSDC |
| **Telegram Integration** | `tg.showAlert`, user ID tracking, mini-app ready |

---

## Gameplay  

### Space Shooter Mode (`#gameContainer`)  
**Objective**: Survive waves, destroy enemies, defeat bosses, earn score & resources.  

#### Controls  
| Platform | Move Left | Move Right | Fire |
|--------|----------|-----------|------|
| **Mobile** | ◀ Button / Left Zone | ▶ Button / Right Zone | **FIRE** Button |
| **Desktop** | `←` | `→` | `Spacebar` |

#### Power-Ups  
| Symbol | Name | Effect | Duration |
|-------|------|-------|----------|
| **S** | Shield | Blocks 1 hit | 10s (stackable) |
| **P** | Speed Boost | +50% speed | 10s+ (combo extend) |
| **L** | Laser Mode | Wider, faster bullets | 10s+ |
| **M** | **Mega Shield** | 2-layer shield | 15s+ (boss drop) |

> **Combo System**: Multiple same-type power-ups extend duration and intensity.

#### Enemy Types  
| Type | Behavior | Special |
|------|--------|--------|
| Normal | Basic descent | — |
| **Code-Drone** | Glitch teleport, time dilation on death | Slows game to 40% |
| **Tank** | High HP (5+), slow | HP bar |
| **Splitter** | Splits into 2 minis | Chain reaction |
| **Boss** | Multi-phase, HP bar, pattern attacks | Every ~45s or stage 5 |

#### Advanced Mechanics  
- **Time Dilation**: Activated during overheat or Code-Drone kill  
- **Weapon Overheat**: Visual bar, affects fire rate  
- **Staged Difficulty**: 5 stages with new enemy types  
- **Boss Phases**: Fan → Spiral → Chaos  

---

### Galactic Strategy Mode (`#galaxyContainer`)  
**Objective**: Expand control, mine resources, complete missions, earn **$XSDC**.  

#### Resources  
| Icon | Name | Use |
|-----|------|-----|
| ⚡ | **Energy** | Primary currency |
| 🪐 | **Metals** | Crafting |
| 💎 | **Crystals** | Rare upgrades |
| 🪙 | **$XSDC** | Prestige token |

> **Passive Mining**: 1% of Energy every **3.5 seconds** while in map mode.

#### Sectors  
| Status | Color | Action |
|-------|-------|--------|
| **Controlled** | Green/Blue | Owned |
| **Enemy** | Red/Pink | Attack via shooter |
| **Neutral** | Gray/Blue | Capture |
| **Mission (Locked)** | Dashed Blue | Requires $XSDC |
| **Mission (Unlocked)** | Pulsing Magenta | **$XDUST-9001** |

#### Special Events  
| Event | Trigger | Reward |
|------|--------|--------|
| **$XDUST-9001** | First visit | **+3141 $XSDC** |
| **Cosmic Mystery** | 16% on map load | **1000–3000 Energy + 888–1776 $XSDC** |
| **Hhaas Event** | Rare | TBD |

---

## Upgrade System (`openUpgradeShopModal`)  

| Upgrade | Max Level | Cost (per level) | Effect |
|--------|-----------|------------------|--------|
| **Fire Rate** | 5 | Energy/Metals/Crystals | Reduces cooldown: `250 / (1 + level×0.15)` ms |
| **Bullet Damage** | 5 | ↑ | `1 + level×0.5` multiplier |
| **Hull Strength** | 3 | ↑ | `+1 life` per level (max 6 lives) |

> **Multi-resource cost** — all three resources required per level.

---

## File Structure  
```
spacedust/
├── xdgame.html          # Full game (self-contained)
├── shoot.mp3            # (Optional) Shooting SFX
├── explosion.mp3        # (Optional) Explosion SFX
├── powerup.mp3          # (Optional) Power-up SFX
└── stardust.png         # (Optional) Galaxy texture
```

---

## How to Play  

1. **Start** → Click **START**  
2. **Shooter Mode** → Survive, collect power-ups, defeat boss  
3. **Galaxy Map** → Click **🌌** to switch  
4. **Capture Sectors** → Enter shooter mode to clear enemies  
5. **Mine & Upgrade** → Spend resources in **🛠️ Upgrades**  
6. **Find $XDUST** → Unlock **$XDUST-9001** for **3141 $XSDC**  
7. **Repeat** → Build your empire!

---

## Technical Highlights  

### Canvas Rendering  
- 60 FPS gameplay loop  
- Particle system (explosions, trails, glitches)  
- Dynamic gradients & shadows  

### Performance  
- Object pooling (bullets, particles)  
- Efficient collision detection  
- Adaptive canvas scaling  

### Telegram Web App  
```js
if (typeof tg !== "undefined") {
    tg.showAlert("Mission Complete! +3141 $XSDC");
}
```
- Safe area insets (`env(safe-area-inset-top)`)  
- Touch-optimized UI  
- No scroll, no selection  

### Data Persistence  
```js
localStorage.setItem('xdust_save_data', JSON.stringify(state));
```
- Saves: Resources, $XSDC, upgrades, score, Telegram ID  

---

## Customization  

Edit these in `<script>`:  
```js
// Difficulty
let enemySpawnRate = 0.03;
let bossInterval = 45000;

// Player
player.speed = 5;

// Power-ups
const COMBO_DURATION = 5000;

// Mining
setInterval(mining, 3500); // 1% energy
```

---

## Tips for Success  

- **Stack Shields** before boss  
- **Use Time Dilation** in tight spots  
- **Prioritize Fire Rate** early  
- **Visit $XDUST-9001 ASAP**  
- **Switch to Galaxy** to mine safely  
- **Save $XSDC** for missions  

---

## Known Issues  

- Audio files **not embedded** (must be added)  
- Some mobile browsers may mute sound until interaction  
- Galaxy map sectors not fully implemented (JS truncated)  
- No cloud sync (localStorage only)  

---

## Support  

- Open browser **DevTools → Console** for errors  
- Ensure **modern browser** (Chrome/Firefox/Safari)  
- For Telegram: Use **official Telegram app**  

---

## License  

**Free to use, modify, and distribute.**  
Attribution appreciated: `By 0penAGI 

---

**Ready to conquer the cosmos?**  
**Launch SPACEDUST and claim your $XSDC!**  

---  
> **"From Dust to Dominion."**  
> **— SPACEDUST Command**
