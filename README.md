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
- 🎲 **Cheat Codes**: Multiple cheat codes available (NETRUNNER, FLATLINE, TRACEBACK) with special abilities
- ⏪ **Undo/Redo System**: Undo and redo moves with TRACEBACK cheat code, works with autodrive mode
- 🔗 **Crosslink Tiles**: Merge all matching pairs and arrange tiles in snake pattern when game is about to end
- 🎨 **Material Icons**: Modern Material Design icons throughout the interface for a polished look
- 🗑️ **Clear High Score**: Reset your high score with a confirmation modal
- 🎨 **Enhanced Tile Visuals**: Gradient depth effects, border glow, and top highlights for 3D appearance
- ✨ **Bevel Text Effect**: Numbers on tiles feature a raised bevel effect for depth
- 📱 **Fully Responsive**: Optimized for desktop, mobile portrait, and landscape orientations
- 💾 **Local Storage**: High score and preferences persistence (sound, difficulty, autodrive speed)
- ⚡ **Glitch Effects**: Cyberpunk-style visual effects on interactions
- 🍎 **iOS Home Screen Support**: Add to home screen with custom PNG icon and app-like experience
- 🎮 **Touch Optimized**: Large touch targets and swipe gestures for mobile gameplay
- 🎯 **Smart Menu System**: Easy-to-access menu with difficulty, sound, cheat, and help options

## 🎮 How to Play

1. Use **arrow keys** or **swipe** (on mobile) to move tiles
2. When two tiles with the same number touch, they **merge into one**
3. Try to create a tile with the number **2048**!
4. Click **REBOOT** to restart the game (reloads page to fetch latest version)
5. Click **Autodrive** to watch the AI play automatically
6. **Sound toggle** (♪ icon): Click the sound icon next to the menu to enable/disable sounds
7. **Undo/Redo** (⏪ ⏩ icons): Available when TRACEBACK cheat is activated - undo or redo your moves
8. Open the **menu** (☰) to access:
   - **Clear High Score**: Reset your high score (with confirmation)
   - **Difficulty**: Select Easy (4x4), Normal (5x5), or Hard (6x6) from the modal
   - **Cheat**: Enter cheat codes to activate special abilities (NETRUNNER, FLATLINE, TRACEBACK)
   - **Help**: View game instructions
9. Control **Autodrive speed** with the slider (0.5x - 5x) when Autodrive is active
10. Double-click/tap the speed value (e.g., "1x") to reset to normal speed
11. Press **Escape** key to close any open modal
12. Click/tap anywhere outside modals to close them
13. The game automatically redraws tiles when the window is resized
14. When **TRACEBACK** is active and the game is about to end, choose from three options:
    - **TRACEBACK**: Undo your last move
    - **CROSSLINK TILES**: Merge all matching pairs (lowest to highest) and arrange remaining tiles in snake pattern
    - **ACCEPT FATE**: Proceed to game over screen

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

Difficulty can be changed from the menu, and your preference is saved to localStorage and persists across sessions.

## 🎲 Cheat Codes

Activate special abilities by entering cheat codes in the cheat menu:

- **NETRUNNER**: Enter this code (case-insensitive) to activate cheat mode
  - Once activated, click or tap any tile to double its value
  - Perfect for testing strategies or reaching higher scores
  - Cheat mode resets when you restart the game

- **FLATLINE**: Enter this code to activate the flatline cheat
  - A red "FLATLINE" button will appear in the cheat menu
  - Click the button to immediately end the game (trigger game over)
  - Useful for testing the game over screen or ending a game quickly

- **TRACEBACK**: Enter this code to activate the undo/redo system
  - Undo and redo buttons (⏪ ⏩) will appear next to the sound icon
  - Click undo to revert your last move, or redo to restore a move you undid
  - Works with both manual moves and autodrive mode
  - When the game is about to end (flatline), a modal will appear with three options:
    - **TRACEBACK**: Undo your last move (turns off autodrive if active)
    - **CROSSLINK TILES**: Automatically merge all matching pairs from lowest to highest (e.g., 2+2→4, 4+4→8, 8+8→16), then arrange remaining tiles in a snake pattern starting from bottom-left and moving right. All merge points are added to your score.
    - **ACCEPT FATE**: Proceed to game over screen
  - If you choose TRACEBACK or CROSSLINK TILES during autodrive, autodrive will automatically turn off
  - Perfect for experimenting with different strategies and learning optimal moves
  - Undo stack is limited to the last 50 moves to prevent memory issues

Access the cheat menu from the main menu (☰) → **⌨️ CHEAT**.

## 🤖 Autodrive Mode

The Autodrive AI uses an advanced heuristic algorithm that:

- **Snake Pattern Strategy**: Keeps the highest tile in the bottom-left corner and builds in a snake pattern upward
- **Corner Strategy**: Maintains the highest tile in the bottom-left corner
- **Smart Merging**: Prioritizes moves that create merges
- **Monotonic Ordering**: Maintains decreasing values from bottom-left to top-right
- **Game-Over Prevention**: Avoids moves that lead to dead ends
- **Direction Preference**: Favors down and left moves for optimal positioning
- **Smoothness Bonus**: Encourages smooth transitions and pattern maintenance

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
- **PNG Icon Support**: Multiple icon sizes (180x180, 152x152, 120x120, 76x76) for optimal iOS display
- **Google Fonts**: Share Tech Mono and Sixtyfour fonts
- **Material Icons**: Google Material Icons for modern UI elements
- **AI Algorithm**: Heuristic-based evaluation function with weighted scoring and snake pattern strategy
- **Dynamic Font Scaling**: Large numbers (6+ digits) automatically scale to fit within tiles
- **Canvas Resize Handling**: Automatic tile redraw on window resize and orientation change
- **Modal System**: Custom-styled modals with backdrop blur and smooth animations
- **Confirmation Dialogs**: Custom confirmation modals matching the cyberpunk theme
- **Undo/Redo System**: State management with undo/redo stacks, works seamlessly with autodrive mode
- **State Persistence**: Game states are saved before each move for undo functionality (limited to 50 moves)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Based on the original [2048 game](https://github.com/gabrielecirulli/2048) by Gabriele Cirulli
- Cyberpunk aesthetic inspired by [Cyberpunk 2077](https://www.cyberpunk.net/) and classic sci-fi themes
- Fonts: [Share Tech Mono](https://fonts.google.com/specimen/Share+Tech+Mono) and [Sixtyfour](https://fonts.google.com/specimen/Sixtyfour)

## 📁 Project Structure

```
cyberpunk-2048/
├── index.html          # Main game file (HTML, CSS, JavaScript)
├── images/            # Icon files
│   ├── 2048-logo.png  # Main app icon
│   └── icon-*.png     # iOS home screen icons (various sizes)
├── README.md          # This file
└── LICENSE           # MIT License
```

## 🎯 Future Enhancements

- [ ] **Achievement System**: Unlock achievements for milestones (reach 512, 1024, 2048, etc.)
- [ ] **Statistics Tracking**: Track total games played, best streak, average score, and move count
- [ ] **Replay System**: Save and replay your best games move-by-move
- [ ] **Multiplayer Mode**: Compete with friends in real-time or turn-based matches
- [ ] **Daily Challenges**: Unique daily puzzles with special objectives or constraints
- [ ] **Time Attack Mode**: Race against the clock to reach 2048 as fast as possible
- [ ] **Power-up System**: Temporary boosts like "Freeze" (skip next spawn) or "Shuffle" (rearrange tiles)
- [ ] **Custom Board Sizes**: Allow players to create custom grid sizes (3x3 to 8x8)
- [ ] **Tile Skins**: Unlockable visual themes for tiles (matrix, neon, holographic, etc.)
- [ ] **Sound Theme Packs**: Different sound sets (synthwave, chiptune, ambient, etc.)
- [ ] **Background Themes**: Multiple cyberpunk environment backgrounds (cityscape, space, data stream)
- [ ] **Gesture Shortcuts**: Custom swipe patterns for quick actions (double-swipe for undo, etc.)
- [ ] **Export/Import Saves**: Share game states or high scores with friends via codes
- [ ] **AI Difficulty Levels**: Different AI personalities for autodrive (aggressive, conservative, random)
- [ ] **Particle Customization**: Adjustable merge particle effects and colors
- [ ] **Accessibility Features**: High contrast mode, reduced motion, and screen reader support
- [ ] **Offline PWA**: Full Progressive Web App with offline support and install prompts
- [ ] **Global Leaderboard**: Online leaderboard with authentication and social features

---

**Enjoy the game!** 🚀✨

