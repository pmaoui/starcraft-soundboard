# StarCraft Original - Soundboard

An interactive web-based soundboard featuring 644 sound effects and quotes from the original StarCraft game (1998).

🎮 **[Live Demo](https://pmaoui.github.io/starcraft-soundboard/)**

![StarCraft Soundboard](https://upload.wikimedia.org/wikipedia/commons/0/0a/StarCraft_Logo.png)

## ✨ Features

- **644 sounds** organized by race (Terran, Zerg, Protoss, and Misc)
- **Play sounds** directly in your browser with visual progress bar
- **Download** individual sounds as MP3 files
- **Filter by race** with intuitive tabs and race icons
- **Keyboard shortcuts** - Press T, Z, P, or M to switch races
- **Authentic StarCraft theme** - Dark interface with race-specific colors
- **Responsive design** - Works on desktop and mobile devices
- **No dependencies** - Pure HTML/CSS/JavaScript

## 🎨 Design

The soundboard features an authentic StarCraft aesthetic:
- **Terran**: Green (#00FF00)
- **Zerg**: Purple (#FF00FF)
- **Protoss**: Cyan (#00D4FF)
- **Misc**: Orange (#FFAA00)

Custom fonts:
- **StarCraft font** for branding
- **Eurostile Extended** for UI elements

## 🚀 Usage

### Online
Visit the live soundboard at: **https://pmaoui.github.io/starcraft-soundboard/**

### Local
1. Clone this repository
2. Open `index.html` in your browser
3. No build process or server required!

### Keyboard Shortcuts
- **T** - Switch to Terran sounds
- **Z** - Switch to Zerg sounds
- **P** - Switch to Protoss sounds
- **M** - Switch to Misc sounds

## 📁 Project Structure

```
Starcraft_Soundboard/
├── index.html              # Main soundboard application
├── README.md              # This file
├── fonts/                 # Custom fonts
│   ├── Starcraft Normal.ttf
│   └── Eurostile Extended Regular/
└── sounds/                # All audio files
    ├── Terran/           # 172 Terran sounds
    ├── Zerg/             # 157 Zerg sounds
    ├── Protoss/          # 214 Protoss sounds
    └── Misc/             # 101 miscellaneous sounds
```

## 🛠️ How It Was Made

This project was created with the assistance of **Claude (Anthropic)** through the Kiro CLI interface. The development process involved:

### Tools & Technologies Used:

1. **Audio Processing**:
   - `ffmpeg` - For audio extraction, splitting, and metadata management
   - Silence detection algorithm to automatically split the original audio file

2. **Speech Recognition**:
   - **OpenAI Whisper** (base model) - For automatic transcription and naming of voice clips
   - Note: Some sound names may be imperfect due to audio quality or background noise

3. **Audio Splitting**:
   - Custom Python scripts using `ffmpeg`'s `silencedetect` filter
   - Threshold: -40dB, minimum silence duration: 0.3s
   - Some sounds may contain multiple clips due to splitting limitations

4. **Web Development**:
   - Pure HTML5, CSS3, and vanilla JavaScript
   - No frameworks or build tools required
   - Self-contained single-page application

5. **Fonts**:
   - StarCraft Normal font for branding
   - Eurostile Extended Regular for UI text

## 📝 Sound Naming

Sounds are automatically named based on their content:
- **Speech clips**: Named after the transcribed quote (e.g., "not_enough_minerals.mp3")
- **Sound effects**: Named as "sfx_###.mp3"

All files include metadata:
- **Title**: Sound name
- **Album**: "Starcraft (Original) - Game sounds"
- **Artist**: Race name (Terran, Zerg, Protoss, or Misc)

### Known Issues

⚠️ **Some sound names may be inaccurate** - The automatic transcription using OpenAI Whisper may have misheard or misinterpreted some audio clips, especially:
- Background noise or music
- Overlapping sounds
- Non-English phrases
- Technical sound effects

⚠️ **Some files contain multiple sounds** - Due to limitations in the silence detection algorithm, a few audio files may contain 2-3 sounds instead of being split into separate files.

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

### Sound Improvements
- **Fix incorrect names** - If you notice a sound is misnamed, please submit a PR with the correct name
- **Split combined sounds** - Some files contain multiple sounds that should be separated
- **Add missing sounds** - If you have additional StarCraft sounds, feel free to add them

### Code Improvements
- **UI/UX enhancements** - Improve the interface or add new features
- **Performance optimizations** - Make the soundboard faster or more efficient
- **Mobile experience** - Enhance the mobile layout and interactions
- **Accessibility** - Add ARIA labels, keyboard navigation improvements, etc.

### How to Contribute
1. Fork this repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test thoroughly
5. Commit your changes (`git commit -m 'Add some improvement'`)
6. Push to the branch (`git push origin feature/improvement`)
7. Open a Pull Request

## 📜 Credits

- **Original game sounds** © Blizzard Entertainment
- **Soundboard development** - Created with assistance from Claude (Anthropic)
- **Audio processing** - ffmpeg, OpenAI Whisper
- **Fonts** - StarCraft font, Eurostile Extended

## ⚖️ License

This is a fan project created for educational and archival purposes. All StarCraft content, including sounds, logos, and trademarks, belong to **Blizzard Entertainment**.

This soundboard is not affiliated with, endorsed by, or sponsored by Blizzard Entertainment.

## 🎮 Enjoy!

Feel free to use this soundboard for:
- Gaming streams
- Discord soundboards
- Nostalgia trips
- StarCraft tournaments
- Personal entertainment

**For Aiur! En Taro Adun!** ⚡
