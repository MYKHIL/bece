# Quick Start Guide

## Getting Started in 5 Minutes

### 1️⃣ Open the App
- Open `index.html` in your web browser
- No installation needed!

### 2️⃣ Wait for Questions to Load
- The app automatically scans for question files
- Shows loading progress in a popup
- Wait for questions to finish loading

### 3️⃣ Select a Subject (Optional)
- If multiple subjects are available, you'll see a dropdown menu
- Select your subject or choose "All Subjects"
- The question count will update

### 4️⃣ Configure Your Session
- **Adjust Settings** (click the gear icon):
  - Number of questions (1-100+)
  - Randomize order (Yes/No)
  - Enable/disable text-to-speech reader
- These settings save automatically

### 5️⃣ Start Studying
- Click **"Start Session (X Qs)"** button
- Answer each question
- Get instant feedback with explanations
- Progress tracker shows your completion

---

## Main Features at a Glance

### 📚 Study Session
```
Question → Select Answer → Check Answer → View Feedback → Next Question
```

### 🎤 Text-to-Speech (Reader)
- Click **"Reader ON"** or **"Reader OFF"** button
- Adjust voice, speed, and pitch in Settings
- Test voice before using

### 📊 Progress Tracking
- **Session History**: View all past attempts
- **Progress Graph**: Visual improvement over time
- **Statistics**: Average, best, worst scores

### 🔄 Review Mode
- After completing a session, click **"Review Questions"**
- See all questions and your answers
- Study explanations in detail

---

## File Organization

### Where to Put Questions
Place question files in this structure:
```
default-questions/
├── Math/
│   └── set1.json (Math questions)
├── Science/
│   └── set1.json (Science questions)
├── English/
│   └── set1.json (English questions)
└── [other subjects]/
    └── set1.json
```

### Question File Format
```json
[
  {
    "id": 1,
    "question": "Your question here",
    "options": {
      "A": "Option 1",
      "B": "Option 2",
      "C": "Option 3",
      "D": "Option 4"
    },
    "answer": "B",
    "explanation": "Why B is correct"
  }
]
```

---

## Tips for Best Experience

✅ **Do This**
- Use Chrome for best compatibility
- Keep questions clear and concise
- Include detailed explanations
- Use LaTeX for mathematical notation ($\frac{1}{2}$)
- Test MathJax rendering locally first

❌ **Don't Do This**
- Don't clear browser cache (you'll lose data)
- Don't delete the index.html file
- Don't modify the app without backup
- Don't leave questions incomplete

---

## Using Text-to-Speech (Reader)

1. Go to **Settings** tab
2. Enable **"Enable Reader"**
3. Choose a **Voice** from dropdown
4. Click **"Test Voice"** to hear it
5. Adjust **Rate** (speed) and **Pitch** (tone)
6. Click **"Start Session"** to hear questions read aloud

---

## Adding Your Own Questions

### Quick Method
1. Save your question file as JSON
2. Place in appropriate subject folder
3. Refresh the page
4. Your questions appear automatically!

### Detailed Steps
1. Create a file named `set2.json`
2. Format with proper JSON structure
3. Include all required fields (id, question, options, answer, explanation)
4. Save to: `default-questions/[Subject]/set2.json`
5. Open app and select subject
6. New questions appear in dropdown!

---

## Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Select Option A | A or 1 |
| Select Option B | B or 2 |
| Select Option C | C or 3 |
| Select Option D | D or 4 |
| Check Answer | Enter |
| Next Question | Right Arrow / N |
| Previous Question | Left Arrow / P |

---

## Troubleshooting

### App Won't Load
- Refresh the page
- Clear browser cache
- Try a different browser
- Check internet connection

### Questions Not Showing
- Verify JSON files are in correct folder
- Check JSON is valid (use JSONLint)
- Ensure folder name matches subject list
- Refresh page after adding files

### Text-to-Speech Not Working
- Enable Reader in Settings
- Check browser permissions
- Try different voice
- Use Chrome for best support

### Math Equations Not Displaying
- Wrap equations in `$...$` for inline
- Wrap in `$$...$$` for block
- Use proper LaTeX syntax
- Refresh page if display is stuck

---

## Common Math Notation Examples

```
Fraction: $\frac{2}{3}$
Mixed: $\frac{1}{2} + \frac{1}{3}$
Power: $x^2 + y^2$
Square Root: $\sqrt{16}$
Scientific: $3.4 \times 10^{-5}$
Subscript: $H_2O$
```

---

## Data Storage

- ✅ **Stored Locally**: Questions, settings, history
- ✅ **Private**: No external servers
- ✅ **Safe**: No personal data collected
- ⚠️ **Note**: Clearing cache will delete stored data

### Backup Your Progress
Export from Management tab:
1. Go to **Management**
2. Click **"Download Current Quiz"**
3. Save JSON file to your computer

---

## Support & Help

- 📖 Read full [README.md](README.md)
- 🤝 See [CONTRIBUTING.md](CONTRIBUTING.md) for adding questions
- 📝 Check [DESCRIPTION.md](DESCRIPTION.md) for technical details
- 📞 Contact: 0542410613

---

## Next Steps

1. ✅ Open index.html
2. ✅ Load some questions
3. ✅ Take a practice quiz
4. ✅ Check Settings (adjust TTS if needed)
5. ✅ View progress on Leaderboard
6. ✅ Add your own questions!

---

**Happy Learning! 🎓**

For detailed information, see the [README.md](README.md) file.
