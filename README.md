# 🏃 Urban Runner

A fast-paced HTML5 canvas game where you run, jump, and collect power-ups while avoiding obstacles in an urban environment.

<img width="953" alt="image" src="https://github.com/user-attachments/assets/e7ae442c-b430-44c8-98f2-593c860ea2ed" />


## ✨ Features

### Core Gameplay
- 🎮 Simple one-button controls (Space/Touch)
- 🏃‍♂️ Auto-running gameplay
- 🦘 Jumping mechanics with double-jump power-up
- 📈 Progressive difficulty
- 🎯 Score and combo system

### Power-ups System
- ⚡ Speed Boost: Increases running speed
- 🔄 Double Jump: Enables mid-air jumps
- 🌟 Invincibility: Temporary immunity to obstacles
- 🧲 Magnet: Attracts nearby coins

### Visual Elements
- 🏙️ Dynamic urban background with scrolling buildings
- 🎨 Customizable character colors
- ✨ Particle effects for collections
- 📊 Visual power-up indicators
- 🏆 High score display

### Technical Features
- 💾 Local storage for high scores
- 📱 Mobile-friendly with touch controls
- 🖥️ Responsive canvas sizing
- 🎯 Collision detection system
- 🔄 Combo multiplier system

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/waleedmustafa971/urban-runner.git
```

2. Navigate to the project directory:
```bash
cd urban-runner
```

3. Open `index.html` in a web browser or serve using a local server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server
```

## 🎮 How to Play

1. **Starting the Game**
   - Press the "Start Game" button or Space bar
   - Touch the screen on mobile devices

2. **Controls**
   - 🔵 Press Space to jump (Desktop)
   - 📱 Tap screen to jump (Mobile)
   - 🔄 Double tap/press for double jump (when power-up is active)

3. **Scoring System**
   - Base points for survival time
   - Coin collection with combo multiplier
   - Power-up bonuses

4. **Power-ups Guide**
   | Power-up | Symbol | Effect | Duration |
   |----------|---------|---------|-----------|
   | Speed Boost | ⚡ | 1.5x speed | 5 seconds |
   | Double Jump | 🔄 | Mid-air jump | 10 seconds |
   | Invincibility | 🌟 | Obstacle immunity | 5 seconds |
   | Magnet | 🧲 | Coin attraction | 7 seconds |

5. **Obstacles**
   - Regular ground obstacles
   - Random spawn patterns
   - Increasing frequency with score

## 🎯 Game Objects Reference

### Player Character
```javascript
const player = {
    x: 100,
    y: CANVAS_HEIGHT - GROUND_HEIGHT,
    width: 40,
    height: 60,
    velocityY: 0,
    isJumping: false,
    color: currentCharacterColor,
    magnetRadius: 100
};
```

### Power-up Types
```javascript
const POWERUP_TYPES = {
    SPEED_BOOST: 'speed',
    DOUBLE_JUMP: 'jump',
    INVINCIBILITY: 'invincible',
    MAGNET: 'magnet'
};
```

## 🔧 Customization

### Character Colors
The game includes 4 default character colors:
- 💚 Green (`#00ff00`)
- ❤️ Red (`#ff0000`)
- 💙 Blue (`#0000ff`)
- 💛 Yellow (`#ffff00`)

To add new colors, modify the `characterColors` array:
```javascript
const characterColors = ['#00ff00', '#ff0000', '#0000ff', '#ffff00'];
```

### Game Constants
Adjust these values to modify game difficulty:
```javascript
const GRAVITY = 0.5;
const JUMP_FORCE = -12;
const COIN_VALUE = 10;
const COMBO_MULTIPLIER = 1.5;
```

## 🔍 Code Structure

```
urban-runner/
├── index.html          # Main game file
├── README.md           # Documentation
└── assets/
    └── sounds/         # (Future addition)
```

### Key Components
- 🎮 Game Loop System
- 🎨 Rendering Engine
- 🔄 Update Logic
- 💥 Collision Detection
- 🎯 Power-up Management
- 💾 Score Tracking
- 🏆 High Score System

## 🔜 Future Enhancements

1. 🎵 Sound System
   - Background music
   - Effect sounds
   - Volume controls

2. 🎨 Visual Improvements
   - Character animations
   - Better obstacle designs
   - Background parallax

3. 📱 Additional Features
   - Achievement system
   - Daily challenges
   - Different game modes

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch:
```bash
git checkout -b feature/amazing-feature
```
3. Commit your changes:
```bash
git commit -m '✨ Add amazing feature'
```
4. Push to the branch:
```bash
git push origin feature/amazing-feature
```
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Inspired by classic runner games
- Built with vanilla JavaScript and HTML5 Canvas
- Special thanks to contributors and testers

## 🐛 Known Issues

- None currently reported

## 📞 Contact

X - [@0x000waleed](https://twitter.com/0x000waleed
)

Project Link: [https://github.com/waleedmustafa971/urban-runner](https://github.com/waleedmustafa971/urban-runner)
