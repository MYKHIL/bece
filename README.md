# MYKHIL's BECE Study Guide

An interactive, modern web-based study platform designed specifically for BECE (Basic Education Certificate Examination) students in Ghana. This application provides immediate feedback quizzes with built-in text-to-speech support, progress tracking, and comprehensive performance analytics.

## 🌟 Features

### Core Functionality
- **Subject-Based Learning**: Organized study materials by subject (Math, Science, English, Social Studies, RME, Computing, Career Technology, and Creative Arts)
- **Immediate Feedback Mode**: Get instant explanations after answering each question
- **Customizable Sessions**: Choose number of questions (1-100+), randomize order, or study sequentially
- **Question Management**: Upload custom quiz files or use pre-loaded question sets

### Advanced Features
- **Text-to-Speech (Reader)**: Built-in native TTS with adjustable voice, rate, and pitch
- **Progress Tracking**: View complete session history with timestamps
- **Performance Analytics**: Visual progress graphs and leaderboard with statistics (average, best, worst scores)
- **Question Navigation**: Quick jump to any question with visual indicators (current, answered, unanswered)
- **Review Mode**: Review all questions and explanations after completing a session
- **Mathematical Expression Rendering**: Full LaTeX support for fractions, scientific notation, superscripts, subscripts, and complex mathematical notation via MathJax

### Mathematical Support
The application uses **MathJax** to render mathematical expressions:
- Fractions: $\frac{2}{3}$
- Scientific Notation: $3.4 \times 10^{-5}$
- Superscripts & Subscripts: $x^2$, $H_2O$
- Complex Equations: All LaTeX format supported

## 📋 System Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- No installation required - runs entirely in the browser
- Internet connection recommended for TTS and MathJax rendering

## 🚀 Getting Started

### Quick Start
1. Clone this repository or download the files
2. Open `index.html` in your web browser
3. The application will automatically scan for question files in the `default-questions` folder
4. Select a subject and start studying!

### File Structure
```
BECE Study Guide Webpage/
├── index.html                 # Main application file (single-page app)
├── default-questions/         # Question storage folder
│   ├── Math/
│   │   └── set1.json         # Math questions
│   ├── Science/
│   │   └── set1.json         # Science questions
│   ├── English/
│   │   └── set1.json         # English questions
│   └── [other subjects]/
├── README.md                  # This file
├── LICENSE                    # MIT License
├── CONTRIBUTING.md            # Contribution guidelines
└── .gitignore                # Git ignore rules
```

## 📊 Question File Format

Questions are stored in JSON format. Each file should contain an array of question objects:

```json
[
  {
    "id": 1,
    "question": "What is $\\frac{2}{3} + \\frac{1}{6}$?",
    "options": {
      "A": "Option text here",
      "B": "Another option",
      "C": "Third option",
      "D": "Fourth option"
    },
    "answer": "B",
    "explanation": "Detailed explanation with $LaTeX$ if needed."
  }
]
```

### Field Descriptions
- **id**: Unique identifier (number)
- **question**: Question text (supports LaTeX with `$...$` for inline or `$$...$$` for block math)
- **options**: Object with keys A-D containing option text
- **answer**: Correct answer key (A, B, C, or D)
- **explanation**: Detailed explanation of the answer
- **subject** (optional): Subject tag (auto-populated by system)

### Text Formatting in Questions
- **Bold text**: Use `**text**` or `*text*` or `'text'`
- **Mathematical expressions**: Use LaTeX syntax within `$...$`
- **Line breaks**: Automatically added before list items (A., B., I., II., 1., etc.)

## 🎮 Usage Guide

### Study Mode
1. **Select Subject** (if available): Choose from available subjects with questions
2. **Configure Settings**: 
   - Set number of questions per session
   - Enable/disable randomization
   - Toggle text-to-speech
3. **Start Session**: Click "Start Session" to begin
4. **Answer Questions**: Select an option and click "Check Answer"
5. **Review Feedback**: Read the explanation and correct answer
6. **Navigate**: Use Previous/Next or click question numbers to jump around

### Settings
- **Questions per Session**: 1 to total available (adjustable with slider)
- **Randomize Order**: Mix up question order for variety
- **Text-to-Speech**:
  - Enable/Disable Reader
  - Choose voice (depends on browser/system)
  - Adjust playback rate (0.5x to 2x)
  - Adjust pitch (0 to 2)
  - Test voice before using

### Leaderboard & Analytics
- **Session History**: View all past attempts with scores and timestamps
- **Statistics**: Average score, best score, worst score
- **Progress Graph**: Visual representation of improvement over time
- **Clear History**: Reset all session data (irreversible)

## 💾 Data Storage

All user data is stored locally in the browser using **localStorage**:
- Quiz settings (number of questions, TTS preferences)
- Session history and scores
- No data is sent to external servers

## 🔧 Management Features

### Upload Questions
1. Go to "Management" tab
2. Select one or more JSON files
3. Click "Process & Load Questions"
4. New uploads replace existing question data

### Download Options
- **Download Template**: Get a sample question file to use as reference
- **Download Current Quiz**: Export all loaded questions as JSON
- **Reset to Default**: Restore original question data

## 📱 Browser Compatibility

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome  | ✅ Full | Recommended for best compatibility |
| Firefox | ✅ Full | Full support |
| Safari  | ✅ Good | iOS and macOS supported |
| Edge    | ✅ Good | Chromium-based version |
| Opera   | ✅ Good | Full support |

## 🎓 Educational Benefits

- **Self-paced Learning**: Study at your own speed
- **Immediate Feedback**: Understand concepts right away
- **Accessibility**: Text-to-speech helps students with different learning styles
- **Progress Motivation**: Track improvement with analytics and leaderboard
- **Comprehensive Coverage**: Customizable question sets for each subject

## 🛠️ Customization

### Adding New Questions
1. Create a JSON file following the format in `Question File Format` section
2. Place it in the appropriate subject folder (e.g., `default-questions/Math/set2.json`)
3. The application automatically detects and loads it on next visit

### Creating New Subject Folders
1. Add a new folder to `default-questions/` with the subject name
2. Place question JSON files in the folder
3. The subject will appear in the selector automatically

### Modifying Settings
- All UI configurations use Tailwind CSS
- TTS settings can be adjusted in Settings view
- Question navigation layout is responsive (mobile & desktop)

## 🐛 Troubleshooting

### Questions Not Loading
- Verify JSON files are in `default-questions/[Subject]/set#.json` format
- Check browser console for syntax errors
- Ensure JSON is valid (use JSON validator)
- Clear browser cache and refresh

### Text-to-Speech Not Working
- Enable TTS in Settings (if previously disabled)
- Check browser permissions for audio
- Not all voices may be available on all systems
- Try different voice options

### MathJax Not Rendering
- Ensure internet connection (MathJax loads from CDN)
- Check if equations use correct LaTeX syntax
- Wrap equations in `$...$` for inline or `$$...$$` for block
- Refresh the page

### Performance Issues
- Reduce number of questions per session
- Close other browser tabs
- Clear browser cache
- Use a newer browser version

## 📄 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Ways to Contribute
- Add new question sets for any subject
- Improve existing questions or explanations
- Report bugs and suggest features
- Improve documentation
- Translate to other languages

## 👤 Developer

**Mr. Michael Darko**
- School: Ayirebi D/A Basic School 'B'
- District: Akyemansa
- Phone: [0542410613](tel:+233542410613)

## 💝 Support This Project

If you find this tool helpful, please consider supporting the developer:
- **Mobile Money**: [0241899862](tel:+233241899862)
- Star this repository ⭐
- Share with other students and educators
- Report bugs and suggest improvements

## 🎯 Roadmap

### Upcoming Features
- [ ] User authentication and cloud sync
- [ ] Multi-language support
- [ ] Offline mode with service workers
- [ ] Mobile app versions (iOS/Android)
- [ ] Teacher dashboard for class management
- [ ] Question difficulty levels
- [ ] Timed quizzes
- [ ] Performance predictions
- [ ] Integration with Google Classroom

## 📚 Resources

- [MathJax Documentation](https://docs.mathjax.org/)
- [JSON Format](https://www.json.org/)
- [LaTeX Math Guide](https://www.latex-project.org/)
- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

## ⚠️ Disclaimer

This is an educational tool designed to help BECE students prepare for exams. While we strive for accuracy, please verify information with official BECE materials and your teachers.

## 📞 Contact & Feedback

For questions, suggestions, or issues:
- Open an issue on GitHub
- Contact the developer via phone: [0542410613](tel:+233542410613)
- Suggest improvements on the GitHub repository

---

**Last Updated**: November 2025  
**Version**: 1.0.0  
**Status**: Active Development

**Happy Learning! 🎓**
