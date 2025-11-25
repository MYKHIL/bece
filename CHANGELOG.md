# Changelog

All notable changes to MYKHIL's BECE Study Guide will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-11-25

### Added
- Initial release of MYKHIL's BECE Study Guide
- Core quiz functionality with immediate feedback
- Subject-based question organization (Math, Science, English, Social Studies, RME, Computing, Career Technology, Creative Arts)
- Subject selection combobox for filtering questions
- Text-to-Speech (Reader) functionality with voice selection, rate, and pitch controls
- Progress tracking with session history and timestamps
- Performance analytics with average, best, and worst scores
- Visual progress graphs showing score progression over time
- Leaderboard with session history and statistics
- Question review mode for post-quiz analysis
- Question navigation with visual indicators (current, answered, unanswered)
- MathJax integration for mathematical expression rendering:
  - LaTeX support for fractions, scientific notation, superscripts, subscripts
  - Automatic equation rendering in questions, options, and explanations
- Customizable quiz sessions:
  - Adjustable number of questions (1 to available)
  - Random or sequential question order
  - Question randomization option
- Settings management:
  - Save and load user preferences
  - Voice selection and testing
  - TTS rate and pitch adjustment
- Quiz management features:
  - Upload custom question files (JSON)
  - Download quiz templates
  - Export current questions
  - Reset to default questions
- Responsive design for mobile and desktop
- Native localStorage for data persistence
- No backend required - static site
- Browser-based text-to-speech API
- Built with Tailwind CSS for modern UI
- Google Analytics integration

### Technical Details
- Single-page application (SPA)
- Pure JavaScript (ES6+)
- HTML5 and CSS3
- Tailwind CSS framework
- MathJax 3 CDN
- Web Speech API
- localStorage for persistence

### Browser Support
- Chrome (Full support)
- Firefox (Full support)
- Safari (Full support)
- Edge (Full support)
- Opera (Full support)

### Files Included
- index.html (Main application)
- default-questions/ (Question storage folder)
  - Math/set1.json (Sample Math questions)
- README.md (Comprehensive documentation)
- LICENSE (MIT License)
- CONTRIBUTING.md (Contribution guidelines)
- DESCRIPTION.md (Project details)
- package.json (Project metadata)
- .gitignore (Git configuration)
- CHANGELOG.md (This file)

### Known Limitations
- Data stored locally in browser (lost if cache is cleared)
- Requires internet for CDN resources
- TTS availability depends on browser/OS
- No offline mode (planned for future)
- No user authentication (planned for future)

### Documentation
- Comprehensive README with features, usage guide, and troubleshooting
- Contributing guidelines for adding questions and code
- Project description with architecture details
- Inline code comments for complex logic

---

## [Planned for Future Releases]

### v1.1.0 (Q1 2026)
- [ ] User authentication system
- [ ] Cloud data synchronization
- [ ] Export progress reports
- [ ] Question difficulty levels
- [ ] Performance predictions

### v1.2.0 (Q2 2026)
- [ ] Offline mode with Service Workers
- [ ] Timed quizzes with countdown
- [ ] Multi-language support
- [ ] Adaptive difficulty
- [ ] Teacher dashboard

### v2.0.0 (Q3 2026)
- [ ] Mobile app (iOS)
- [ ] Mobile app (Android)
- [ ] Google Classroom integration
- [ ] Advanced analytics
- [ ] Question filtering by difficulty

---

## How to Report Issues

Found a bug or have a feature request? Please:
1. Check existing issues to avoid duplicates
2. Open a new issue with clear description
3. Include steps to reproduce for bugs
4. Provide browser and OS information

## How to Contribute

See CONTRIBUTING.md for detailed guidelines on:
- Adding new questions
- Reporting bugs
- Suggesting features
- Improving code
- Submitting pull requests

---

**Thank you for using and supporting MYKHIL's BECE Study Guide!**
