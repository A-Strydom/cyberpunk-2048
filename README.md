# 🎮 Cyberpunk 2048

A cyberpunk-themed implementation of the classic 2048 puzzle game with stunning neon visuals, smooth animations, and an AI autodrive mode.

![Cyberpunk 2048](https://img.shields.io/badge/Game-2048-00f5ff?style=for-the-badge&logo=gamepad&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## ✨ Features

- 🎨 **Cyberpunk Aesthetic**: Neon cyan, pink, and yellow color scheme with glowing effects
- 🎯 **Smooth Animations**: Fluid tile movements and merge effects
- 🎵 **Musical Sound System**: Pentatonic scale notes for moves and merges, with sound effects for all game events
- 🔊 **Sound Controls**: Enable/disable sounds with persistent preferences
- 🤖 **Intelligent Autodrive Mode**: Advanced AI with bottom-left corner strategy and smart decision-making
- ⚡ **Autodrive Speed Control**: Adjustable speed from 0.5x to 5x with smooth slider control
- 🎚️ **Difficulty Levels**: Easy (4x4), Normal (5x5), and Hard (6x6) modes with dynamic spawn probabilities
- 📱 **Fully Responsive**: Optimized for desktop, mobile portrait, and landscape orientations
- 💾 **Local Storage**: High score and preferences persistence (sound, difficulty, autodrive speed)
- ⚡ **Glitch Effects**: Cyberpunk-style visual effects on interactions
- 🍎 **iOS Home Screen Support**: Add to home screen with custom icon and app-like experience
- 🎮 **Touch Optimized**: Large touch targets and swipe gestures for mobile gameplay

## 🎮 How to Play

1. Use **arrow keys** or **swipe** (on mobile) to move tiles
2. When two tiles with the same number touch, they **merge into one**
3. Try to create a tile with the number **2048**!
4. Click **REBOOT** to restart the game (reloads page to fetch latest version)
5. Click **Autodrive** to watch the AI play automatically
6. Adjust **difficulty** from the dropdown (Easy/Normal/Hard)
7. Toggle **sound** on/off from the menu
8. Control **Autodrive speed** with the slider (0.5x - 5x) when Autodrive is active
9. Double-click/tap the speed value (e.g., "1x") to reset to normal speed

## 🚀 Getting Started

### Local Development

Simply open `index.html` in your web browser. No build process or dependencies required!

### GitHub Pages

This repository is configured for GitHub Pages. The game will be automatically deployed at:
```
https://[your-username].github.io/cyberpunk-2048/
```

To enable GitHub Pages:
1. Go to your repository settings
2. Navigate to "Pages" in the sidebar
3. Select the `main` branch as the source
4. Save and wait for deployment

## 🎵 Sound System

The game features a comprehensive sound system with musical notes and sound effects:

- **Musical Notes**: Moves and merges play notes from a pentatonic scale (C, D, E, G, A, C)
- **Sound Effects**:
  - New tile spawn: Subtle pop sound
  - Invalid move: Low error tone
  - Game over: Descending tone sequence
  - Glitch effect: Distorted multi-tone sound (on REBOOT)
  - Autodrive launch: Hypercar/spaceship launch sound
  - Autodrive stop: Engine shutdown sound
- **Sound Toggle**: Enable/disable sounds via the menu (preference saved to localStorage)
- **Mobile Support**: Audio context automatically resumes on first user interaction

## 🎚️ Difficulty Levels

Choose from three difficulty levels, each with different board sizes and spawn probabilities:

- **Easy**: 4x4 grid, higher probability of spawning 2s
- **Normal**: 5x5 grid, balanced spawn probabilities (default)
- **Hard**: 6x6 grid, higher probability of spawning 4s

Difficulty preference is saved to localStorage and persists across sessions.

## 🤖 Autodrive Mode

The Autodrive AI uses an advanced heuristic algorithm that:

- **Corner Strategy**: Keeps the highest tile in the bottom-left corner
- **Smart Merging**: Prioritizes moves that create merges
- **Monotonic Ordering**: Maintains decreasing values from bottom-left to top-right
- **Game-Over Prevention**: Avoids moves that lead to dead ends
- **Direction Preference**: Favors down and left moves for optimal positioning

### Speed Control

When Autodrive is active:
- Adjust speed from **0.5x** (slow) to **5x** (very fast) using the slider
- Speed preference is saved and persists across sessions
- Double-click/tap the speed value (e.g., "1x") to quickly reset to normal speed
- Stop Autodrive anytime with the stop button (⏹)

## 🎨 Customization

The game uses CSS custom properties and can be easily customized by modifying the color values in the `<style>` section of `index.html`.

### Key Colors
- **Cyan**: `#00f5ff` - Primary accent color (buttons, borders, controls)
- **Pink/Magenta**: `#ff00ff` - Secondary accent color
- **Yellow**: `#ffeb3b` - Highlight color
- **Orange**: `#ff6b35` - Button accent color (REBOOT, Autodrive)

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript**: No frameworks or dependencies
- **Canvas Rendering**: Smooth 60fps animations with optimized rendering
- **Web Audio API**: Programmatic sound generation with AudioContext
- **Local Storage API**: For high score, sound preferences, difficulty, and autodrive speed persistence
- **Debounced Storage**: Optimized localStorage writes to prevent performance issues
- **CSS Filters**: For glow and visual effects
- **Responsive Media Queries**: Support for portrait, landscape, and various screen sizes
- **Touch Events**: Swipe gesture detection for mobile gameplay
- **iOS Meta Tags**: Apple touch icon and web app capabilities for home screen installation
- **Google Fonts**: Share Tech Mono and Sixtyfour fonts
- **AI Algorithm**: Heuristic-based evaluation function with weighted scoring

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Based on the original [2048 game](https://github.com/gabrielecirulli/2048) by Gabriele Cirulli
- Cyberpunk aesthetic inspired by classic sci-fi themes
- Fonts: [Share Tech Mono](https://fonts.google.com/specimen/Share+Tech+Mono) and [Sixtyfour](https://fonts.google.com/specimen/Sixtyfour)

## 🎯 Future Enhancements

- [ ] Theme variations
- [ ] Leaderboard system
- [ ] Additional sound effect options
- [ ] Custom color schemes

---

**Enjoy the game!** 🚀✨

