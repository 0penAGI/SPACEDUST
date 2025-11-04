# SPACEDUST - Space Shooter Game

![SPACEDUST](https://img.shields.io/badge/SPACEDUST-Cosmic%20Shooter-blue?style=for-the-badge&logo=starship)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Mobile](https://img.shields.io/badge/Mobile-Friendly-00ff00?style=flat&logo=smartphone)

## 🎮 About the Game

SPACEDUST is an exciting space shooter game built with pure HTML5, CSS3, and JavaScript. Defend the galaxy against cosmic invaders in this action-packed arcade-style game with stunning visual effects and smooth controls optimized for both desktop and mobile devices.

## ✨ Features

- **🎯 Intuitive Controls**: Touch-optimized controls for mobile and keyboard support for desktop
- **🚀 Power-up System**: Collect various power-ups to enhance your ship
- **👾 Boss Battles**: Epic boss encounters every 45 seconds
- **💥 Visual Effects**: Particle explosions, shield effects, and stunning animations
- **⭐ Dynamic Background**: Parallax starfield with twinkling effects
- **📱 Responsive Design**: Works perfectly on all screen sizes
- **🔊 Sound Effects**: Immersive audio experience (requires sound files)
- **🏆 Scoring System**: Compete for high scores
- **🌌 Galactic Strategy Mode**: Resource management and sector control
- **🛠️ Upgrade System**: Enhance your ship with permanent upgrades
- **💰 XDUST Economy**: In-game currency system with mining mechanics
- **⚡ Time Dilation**: Advanced combat mechanic with overheat system

## 🎯 Gameplay

### Objective
Protect the galaxy by destroying enemy ships and surviving as long as possible. Collect power-ups, defeat the boss, and achieve the highest score!

### Controls
- **Mobile**: Use on-screen buttons for movement and firing
- **Desktop**: Arrow keys for movement, Spacebar for shooting

### Power-ups
- **S (Shield)**: Temporary invincibility for 10 seconds
- **P (Speed)**: Increased movement speed for 10 seconds
- **L (Laser)**: Enhanced weaponry for 10 seconds
- **M (Mega Shield)**: Powerful two-layer shield (boss drop)

## 🛠️ Installation

### Quick Start
1. Download the `index.html` file
2. Place it in your web server directory
3. Add sound files (optional):
   - `shoot.mp3` - Shooting sound
   - `explosion.mp3` - Explosion sound
   - `powerup.mp3` - Power-up collection sound
4. Open in any modern web browser

### Telegram Mini App
The game includes Telegram WebApp integration for use as a Telegram Mini App.

## 🎨 Technical Features

### Graphics
- Canvas-based rendering for smooth performance
- CSS animations for UI elements
- Gradient effects and shadows
- Particle system for explosions

### Performance
- Optimized for 60fps gameplay
- Efficient collision detection
- Memory management for game objects
- Adaptive difficulty scaling

### Compatibility
- **Browsers**: Chrome, Firefox, Safari, Edge
- **Mobile**: iOS Safari, Android Chrome
- **Screen Sizes**: 320px and up

## 📁 File Structure

```
spacedust/
├── index.html          # Main game file
├── shoot.mp3          # Shooting sound effect
├── explosion.mp3      # Explosion sound effect
└── powerup.mp3        # Power-up collection sound
```

## 🎮 Game Mechanics

### Player Ship
- 3 lives at start (upgradable)
- Responsive movement
- Visual damage feedback
- Multiple weapon types
- Time dilation combat system

### Enemies
- Random spawn patterns
- Increasing difficulty over time
- Different sizes and speeds
- Boss enemy with health bar
- Special Code Drone enemies

### Scoring
- **Normal Enemy**: 10 points
- **Power-up Collection**: 50 points
- **Boss Defeat**: 500 points

## 🚀 How to Play

1. **Start**: Click "START" on the main screen
2. **Movement**: Use left/right controls to avoid enemies
3. **Shooting**: Press fire button to destroy enemies
4. **Collect**: Grab power-ups for temporary advantages
5. **Survive**: Avoid enemy collisions and survive as long as possible
6. **Boss Fight**: Defeat the boss that appears every 45 seconds

## 🌌 Galactic Strategy Mode

The game features a comprehensive galactic strategy mode where you can:

- **Manage Resources**: Collect energy, metals, and crystals
- **Control Sectors**: Capture and defend galactic territories
- **Complete Missions**: Special missions with unique rewards
- **Upgrade Technology**: Permanent ship improvements
- **Mine XDUST**: Generate resources over time

### Strategy Features
- **Resource Management**: Balance energy, metals, and crystals
- **Sector Control**: Expand your influence across the galaxy
- **Mission System**: Complete objectives for rewards
- **Upgrade Shop**: Permanent improvements to your ship
- **Achievements**: Track your progress and accomplishments

## 🛠️ Upgrade System

### Available Upgrades
- **Fire Rate**: Decrease shooting cooldown (5 levels)
- **Bullet Damage**: Increase damage output (5 levels)
- **Hull Strength**: Add extra lives (3 levels)

### Economy
- **XDUST**: Main in-game currency
- **Energy**: Primary resource for upgrades
- **Metals**: Crafting material
- **Crystals**: Rare resource for advanced upgrades

## 🎯 Tips for Success

- **Prioritize Power-ups**: They can save you in tight situations
- **Watch for Boss**: Save your shields for boss encounters
- **Stay Mobile**: Constant movement makes you harder to hit
- **Manage Space**: Use the entire screen to your advantage
- **Use Time Dilation**: Strategic slowdown for difficult situations
- **Upgrade Wisely**: Balance offensive and defensive upgrades
- **Complete Missions**: Earn bonus resources and XDUST

## 🔧 Customization

The game can be easily customized by modifying these variables in the JavaScript:

```javascript
// Difficulty settings
let enemySpawnRate = 0.03;
let bossInterval = 45000; // 45 seconds

// Player settings
const player = {
    speed: 5,
    // ... other properties
};

// Power-up durations
// Shield: 10000ms (10 seconds)
// Speed: 10000ms (10 seconds)  
// Laser: 10000ms (10 seconds)
// Mega Shield: 15000ms (15 seconds)

// Time Dilation settings
let timeDilationFactor = 1.0;
let timeDilationMax = 0.5;
```

## 🌟 Special Features

### Visual Effects
- Neon glow effects
- Particle explosions
- Ship damage flashing
- Power-up collection flashes
- Animated engine flames
- Galactic map animations

### Audio Integration
- Three-channel sound system
- Proper audio timing
- Error handling for missing files
- Web Audio API support

### Mobile Optimization
- Touch-friendly controls
- Prevent default browser behaviors
- Optimized performance for mobile devices
- Safe area support for notched displays

### Advanced Mechanics
- **Time Dilation**: Slow down time during intense combat
- **Overheat System**: Manage weapon heat for optimal performance
- **Code Drones**: Special enemy types with unique behavior
- **Resource Streaming**: Animated resource transfers between sectors

## 🐛 Known Issues

- Sound files need to be provided separately
- Some older browsers may have performance issues
- Very small screens might have cramped controls

## 📞 Support

For issues or suggestions:
1. Check browser console for errors
2. Ensure sound files are in correct location
3. Verify modern browser is being used

## 📄 License

This game is free to use and modify. Attribution is appreciated but not required.
By 0penAGI

---

**Ready to defend the galaxy? Launch SPACEDUST and begin your cosmic adventure!** 🚀✨
