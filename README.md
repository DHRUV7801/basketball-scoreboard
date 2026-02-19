# 🏀 Basketball Scoreboard

A simple, interactive basketball scoreboard application built with HTML, CSS, and JavaScript. Keep track of scores for two teams in real-time with a clean, digital-style interface.

## 📋 Table of Contents

- [Demo]
- [Features]
- [Usage]
- [File Structure]
- [Technologies Used]
- [Responsive Design]
- [Contributing]
- [License]
- [Contact]

## 🎮 Demo

<!-- Add your live demo link here -->
[Live Demo](https://d78basketball-scoreboard.netlify.app/)

## ✨ Features

- ⚡ **Real-time Score Tracking** - Update scores instantly with button clicks
- 🎯 **Multiple Point Options** - Add 1, 2, or 3 points per action
- 👥 **Dual Team Support** - Track scores for two teams simultaneously
- 📝 **Custom Team Names** - Enter your own team names before starting
- 🏆 **Winner Declaration** - Automatically determines and announces the winner
- 🔄 **Game Reset** - Reset scores after each game ends
- 📱 **Fully Responsive** - Works seamlessly on mobile, tablet, and desktop
- 🎨 **Digital Display Style** - Classic digital scoreboard aesthetic
- ⚠️ **Input Validation** - Prevents scoring before team names are entered

## 📸 Screenshots

<!-- Add screenshots here -->
```
[Add screenshot of the basketball scoreboard interface]
```

## 🚀 Installation

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required!

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/DHRUV7801/basketball-scoreboard.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd basketball-scoreboard
   ```

3. **Open the application**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js
     npx http-server
     ```

4. **Access the application**
   - Open your browser and go to `http://localhost:8000`

## 💡 Usage

### Getting Started

1. **Enter Team Names**
   - Type the first team's name in the "Team-1" input field
   - Type the second team's name in the "Team-2" input field

2. **Update Scores**
   - Click **+1** to add 1 point (free throw)
   - Click **+2** to add 2 points (regular basket)
   - Click **+3** to add 3 points (three-pointer)

3. **End the Game**
   - Click **"End Game"** button when the match is over
   - The app will automatically:
     - Determine the winner
     - Display the final scores
     - Show an alert with the result
     - Reset both scores to 0

### Example Flow

```
1. Enter "Lakers" for Team 1
2. Enter "Warriors" for Team 2
3. Click +3 for Lakers → Score: 3-0
4. Click +2 for Warriors → Score: 3-2
5. Click +2 for Lakers → Score: 5-2
6. Click "End Game" → "Lakers wins with a score of 5!"
7. Scores reset to 0-0 for next game
```

## 📁 File Structure

```
basketball-scoreboard/
│
├── index.html          # Main HTML structure
├── basket.css          # Styling and responsive design
├── basket.js           # JavaScript functionality
└── README.md           # Project documentation
```

### File Descriptions

- **index.html** - Contains the HTML structure with team inputs, score displays, and control buttons
- **basket.css** - Provides styling with a dark theme, digital font, and responsive layouts
- **basket.js** - Implements all game logic including score updates, validation, and winner determination

## 🛠 Technologies Used

- **HTML5** - Structure and semantic markup
- **CSS3** - Styling, animations, and responsive design
- **JavaScript** - Game logic and interactivity
- **DS-Digital Font** - Classic digital display appearance (via CDN)

## 📱 Responsive Design

The application is fully responsive and optimized for:

### Mobile Devices (< 600px)
- Vertical layout with stacked teams
- Adjusted font sizes for readability
- Touch-friendly button sizes
- Optimized spacing

### Tablets (601px - 1024px)
- Side-by-side team layout
- Medium-sized controls
- Balanced spacing

### Desktop (> 1024px)
- Full-width horizontal layout
- Large digital displays
- Maximum readability

## 🎨 Customization

### Changing Colors

Edit `basket.css` to customize the color scheme:

```css
body {
    background-color: rgb(15, 10, 56);  /* Background */
    color: white;                        /* Text */
}

.screen {
    background-color: rgb(0, 0, 0);     /* Display background */
    color: rgb(126, 20, 20);            /* Score color */
}
```

### Adding More Point Options

Add new buttons in `index.html`:

```html
<button onclick="plus4('team1')">+4</button>
```

And create the function in `basket.js`:

```javascript
function plus4(team) {
    if (!validateTeamNames()) return;
    let screen = document.getElementById(team);
    let currentScore = parseInt(screen.textContent);
    screen.textContent = currentScore + 4;
}
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the project
2. Create your feature branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. Push to the branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request

### Ideas for Contribution

- [ ] Add timer/countdown functionality
- [ ] Implement quarter/period tracking
- [ ] Add sound effects for scoring
- [ ] Create a score history/log
- [ ] Add player statistics tracking
- [ ] Implement dark/light theme toggle
- [ ] Add keyboard shortcuts
- [ ] Create a settings panel
- [ ] Add animations for score changes
- [ ] Implement undo/redo functionality

## 🐛 Known Issues

- None currently reported

## 📝 Future Enhancements

- 🕐 Game timer with periods/quarters
- 📊 Statistics tracking (shooting percentage, fouls, etc.)
- 💾 Save game history
- 🎵 Sound effects and animations
- ⌨️ Keyboard shortcuts for faster scoring
- 🌓 Dark/light theme toggle
- 📤 Export game results
- 🏅 Tournament mode with multiple games

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Dhruv Goyal**

- GitHub: [@DHRUV7801](https://github.com/DHRUV7801)
- LinkedIn: [Dhruv Goyal](https://www.linkedin.com/in/dhruv-goyal-494991313)
- Twitter: [@Dhruvgm78](https://x.com/Dhruvgm78)

## 🙏 Acknowledgments

- DS-Digital font from [CDN Fonts](https://fonts.cdnfonts.com/)
- Inspired by classic basketball scoreboards
- Thanks to all contributors

## 📞 Support

If you have any questions or need help, please:

1. Check the [Issues](https://github.com/DHRUV7801/basketball-scoreboard/issues) page
2. Create a new issue if your problem isn't already listed
3. Contact me via email or social media

---

<div align="center">

**If you found this project helpful, please give it a ⭐!**

Made with ❤️ by Dhruv Goyal

</div>
