# 🎮 Tug of War: Mathematics - Educational Game

A fun and interactive mathematical game designed for children below 10 years to master math skills through an engaging tug-of-war mechanics.

## 🎯 Game Overview

**Tug of War: Mathematics** is a competitive math game where two players (Team A and Team B) compete by solving math problems. Each correct answer pulls the opponent's team towards the center line. The first team to fully pull their opponent past the centerline wins!

### 🏆 How to Play

1. **Settings**: Start by selecting your game preferences:
   - Choose math operations (Addition, Subtraction, Multiplication, Division)
   - Select difficulty level (Easy: 1-10, Medium: 1-20, Hard: 1-50)
   - Set time limit per question (30s - 2 minutes)
   - Choose winning score (3, 5, or 10 points)

2. **Game Screen**:
   - Each team sees a different math question
   - Use the virtual keyboard to input your answer
   - Press ✓ (tick) to submit your answer
   - Use ⌫ (delete) to correct mistakes

3. **Scoring & Movement**:
   - Correct answer = 1 point + rope movement towards your team
   - Wrong answer = No points, rope stays in place
   - First team to reach the winning score pulls the opponent fully to their side

4. **Victory**:
   - Winning team gets a trophy 🏆
   - Celebration with confetti 🎉

## 🎮 Team Identification

### Team A (Left Side)
- **Color**: Blue
- **Attire**: Blue shirt & shoes, black pants
- **Position**: Left side of screen

### Team B (Right Side)
- **Color**: Red  
- **Attire**: Red shirt & shoes, black pants
- **Position**: Right side of screen

## 🕹️ Controls

### Virtual Keyboard (Both Teams)
- **Numbers 1-9, 0**: Input digits
- **✓ (Tick)**: Submit your answer
- **⌫ (Delete)**: Delete last digit

### Game Controls
- **⚙️ Settings Button**: Return to settings (pauses game)
- **Timer**: Shows time remaining for current question

## 🛠️ Features

✅ **Customizable Difficulty**: Easy, Medium, Hard levels
✅ **Multiple Operations**: Addition, Subtraction, Multiplication, Division
✅ **Different Questions**: Each team gets unique questions
✅ **Real-time Timer**: Visual feedback on time remaining
✅ **Score Tracking**: Live points display for both teams
✅ **Rope Animation**: Visual tug-of-war representation
✅ **Player Animations**: Teams pull in sync with correct answers
✅ **Responsive Design**: Works on all screen sizes
✅ **Winner Celebration**: Trophy animation and confetti
✅ **Local Multiplayer**: Perfect for siblings or classroom use

## 🚀 Installation & Usage

### Quick Start

1. **Extract Files**: Place `index.html`, `styles.css`, and `game.js` in the same folder

2. **Open in Browser**: 
   - Double-click `index.html`, OR
   - Right-click → Open with Browser → Select your browser

3. **Configure Game**:
   - Select math operations you want to practice
   - Choose difficulty level
   - Set time per question
   - Choose target score to win

4. **Start Playing**: Click "Start Game 🎮"

### File Structure
```
tug-of-war-math/
├── index.html       (Main game structure)
├── styles.css       (Styling & animations)
├── game.js          (Game logic)
└── README.md        (This file)
```

## 📊 Game Settings Explained

### Difficulty Levels
- **Easy**: Numbers from 1 to 10
  - Great for beginners
  - Recommended for kids 5-7 years
  
- **Medium**: Numbers from 1 to 20
  - Intermediate level
  - Recommended for kids 7-9 years
  
- **Hard**: Numbers from 1 to 50
  - Advanced level
  - Recommended for kids 9+ years or competitive play

### Time Limits
- **30 seconds**: Fast-paced, challenging
- **45 seconds**: Balanced
- **60 seconds** (Default): Relaxed, thinking time
- **120 seconds**: Plenty of time to work through problems

### Scoring to Win
- **3 Points**: Quick game (~5-10 minutes)
- **5 Points** (Default): Standard game (~10-15 minutes)
- **10 Points**: Extended game (~20-30 minutes)

## 🎓 Educational Benefits

✨ **Math Practice**: Improves calculation speed and accuracy
✨ **Competition**: Motivates through friendly competition
✨ **Time Management**: Players learn to work under pressure
✨ **Multiple Operations**: Covers various math concepts
✨ **Engagement**: Fun game format keeps kids interested
✨ **Customizable**: Adjustable difficulty for learning curves

## 💡 Tips for Teachers/Parents

1. **Start Easy**: Begin with Easy difficulty and 60-second time limits
2. **Build Up**: Gradually increase difficulty as skills improve
3. **Mix Operations**: Use all four operations to keep it challenging
4. **Celebrate**: Praise correct answers, encourage learning from mistakes
5. **Group Play**: Can be used for classroom competitions
6. **Regular Practice**: Short 5-10 minute sessions are more effective

## 🔧 Customization

You can modify the game by editing the files:

### Adjust Difficulty Ranges (game.js)
```javascript
case 'easy': return [1, 10];      // Change these numbers
case 'medium': return [1, 20];
case 'hard': return [1, 50];
```

### Change Team Colors (styles.css)
```css
.blue-shirt { background: #1e90ff; }    /* Change hex to different color */
.red-shirt { background: #ff1744; }
```

### Modify Rope Movement Speed
```javascript
const movementAmount = 4;  // Change in updateRopePosition()
```

## ⚠️ Technical Requirements

- **Browser**: Modern web browser (Chrome, Firefox, Safari, Edge)
- **Screen**: At least 1024x768 resolution recommended
- **Input**: Mouse or touchscreen for virtual keyboard
- **Offline**: Game runs completely offline, no internet required

## 🐛 Known Limitations

- Designed for local multiplayer (same device)
- Best played on desktop/tablet screens
- Mobile screens may require landscape orientation
- Works at any screen size but 1920x1080+ recommended for best experience

## 🎨 Design Features

- Beautiful gradient backgrounds
- Smooth animations and transitions
- Clear visual feedback for inputs
- Responsive layout
- Accessible color scheme
- Player character animations
- Trophy and celebration effects
- Turn indicators for clarity

## 📝 Game Flow

```
Settings Screen
      ↓
Select Operations & Difficulty
      ↓
Choose Time & Score Settings
      ↓
Start Game
      ↓
Generate Different Questions for Each Team
      ↓
Players Input Answers Using Virtual Keyboard
      ↓
Check Answers
      ├→ Correct: Award Point + Move Rope
      └→ Wrong: No Point + Continue
      ↓
Check if Someone Won (Reached Target Score)
      ├→ Yes: Show Winner Screen with Trophy
      └→ No: Generate New Questions (Back to Step 4)
      ↓
Play Again or Return to Settings
```

## 🎯 Winning Conditions

A team wins when:
- They reach the target score (3, 5, or 10 points based on settings)
- AND have fully pulled the opponent past the centerline

## 🔄 Game Mechanics

**Rope Position**:
- Starts at 50% (center)
- Each correct answer moves rope 4% toward that team
- 0% = Team B fully pulled, Team A wins
- 100% = Team A fully pulled, Team B wins

**Question Generation**:
- Questions are randomly generated
- Each team always gets different questions
- Operations are randomly selected from chosen operations
- Numbers are within the selected difficulty range

**Timer**:
- Starts with selected time limit
- Counts down in real-time
- Turns yellow at 30 seconds remaining
- Turns red and blinks at 10 seconds
- When time expires, no points awarded, new question appears

## 🎮 Recommended Usage Scenarios

✅ **Classroom**: Group competitions, math practice
✅ **Home**: Sibling rivalries, fun learning
✅ **Tutoring**: Supplement to math lessons
✅ **Summer Learning**: Keep skills sharp during break
✅ **Rainy Day**: Indoor entertainment
✅ **Brain Training**: Regular mental exercise

## 📚 Learning Outcomes

After playing regularly, students should achieve:
- Faster mental math calculations
- Better accuracy in math operations
- Improved focus and concentration
- Enhanced problem-solving under time pressure
- Better understanding of mathematical concepts
- Increased confidence in math abilities

## 🤝 Support & Contributions

For suggestions, improvements, or bug reports, feel free to enhance the game files!

## 📄 License

This game is free to use for educational purposes.

---

**Enjoy Learning Math Through Play!** 🎮📚✨

Created to make mathematics fun and engaging for children.
