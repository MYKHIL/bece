# Contributing to MYKHIL's BECE Study Guide

Thank you for your interest in contributing to this educational project! We welcome contributions from students, teachers, developers, and anyone passionate about improving exam preparation for BECE students.

## 📋 Code of Conduct

Please be respectful and constructive in all interactions. We are committed to providing a welcoming and inclusive environment for all contributors.

## 🤝 How to Contribute

### 1. Add or Improve Questions

The easiest way to contribute is by adding or improving question sets for any subject.

#### Adding New Questions
1. **Create a JSON file** following this format:
```json
[
  {
    "id": 1,
    "question": "Your question text here, can include $LaTeX$ math",
    "options": {
      "A": "First option",
      "B": "Second option",
      "C": "Third option",
      "D": "Fourth option"
    },
    "answer": "B",
    "explanation": "Detailed explanation of why B is correct and why others are wrong."
  }
]
```

2. **Save the file** in the appropriate folder:
   - For new subjects: `default-questions/[SubjectName]/set1.json`
   - For additional questions: `default-questions/[SubjectName]/set2.json`, etc.

3. **Validate your JSON** using a JSON validator before submitting

4. **Test locally** by placing the file in your `default-questions` folder and loading it in the app

5. **Submit a Pull Request** with:
   - Clear description of questions added/improved
   - Number of questions included
   - Subject covered

#### Question Quality Guidelines
- ✅ **Clear and Unambiguous**: Questions should be easily understood
- ✅ **Accurate**: Verify all answers with reliable sources
- ✅ **Detailed Explanations**: Help students understand the concept, not just memorize
- ✅ **Appropriate Difficulty**: Match BECE exam level
- ✅ **Diverse Content**: Cover different aspects of the subject
- ✅ **Proper Formatting**: Use consistent styling and LaTeX for math

### 2. Report Bugs

Found a problem? Help us fix it!

1. **Check existing issues** to avoid duplicates
2. **Create a new issue** with:
   - Clear title describing the problem
   - Steps to reproduce
   - Expected vs actual behavior
   - Browser and OS information
   - Screenshots if relevant

**Example Bug Report**:
```
Title: MathJax not rendering fractions on Firefox

Steps to Reproduce:
1. Open app in Firefox
2. Select Math subject
3. Attempt first question

Expected: Fractions should display properly
Actual: Fractions show as raw LaTeX code

Browser: Firefox 121.0
OS: Windows 11
```

### 3. Suggest Features

Have an idea to improve the app?

1. **Check existing issues** to see if it's already suggested
2. **Open a feature request** with:
   - Clear description of the feature
   - Why it would be helpful
   - How it should work
   - Example use cases

**Example Feature Request**:
```
Title: Add timer/timed quizzes

Description:
Many exams are timed. A timer feature would help students 
practice time management.

Suggested Implementation:
- Add "Timed Mode" option in settings
- Allow selection of time per question or total time
- Show countdown timer during quiz
```

### 4. Improve Documentation

Good documentation helps everyone!

Ways to help:
- Fix typos or unclear explanations
- Add examples to README
- Create troubleshooting guides
- Translate documentation

### 5. Code Contributions

For code changes:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Make your changes** following the code style below
4. **Test thoroughly** before submitting
5. **Commit with clear messages**: `git commit -m "Add/Fix/Improve: description"`
6. **Push to your fork**: `git push origin feature/your-feature-name`
7. **Submit a Pull Request** with detailed description

#### Code Style Guidelines
- Use meaningful variable names
- Add comments for complex logic
- Follow existing code patterns
- Test in multiple browsers
- Keep functions focused and modular
- Avoid global namespace pollution

#### JavaScript Best Practices
- Use `const` by default, `let` for reassignment, avoid `var`
- Use modern ES6+ features where appropriate
- Add error handling with try-catch
- Test text-to-speech and MathJax rendering
- Ensure responsive design works on mobile

### 6. Translation

Help make this tool available in other languages!

1. Create a translation file with the language code
2. Include all UI text, labels, and messages
3. Ensure cultural appropriateness
4. Test with native speakers if possible

## 📝 Pull Request Process

1. **Update documentation** if you've changed functionality
2. **Test your changes** thoroughly
3. **Write a clear PR description** explaining:
   - What problem does this solve?
   - How does it solve it?
   - Any breaking changes?
   - Testing done?

4. **Link related issues** using `Closes #123`
5. **Wait for review** - maintainers will provide feedback
6. **Address feedback** promptly
7. **Squash commits** if requested before merging

## 🎯 Prioritized Contribution Areas

We're especially looking for help with:
1. **Question Sets**: More questions for all subjects, especially:
   - Advanced Math topics
   - Science practicals
   - English comprehension passages
   - Historical dates and events
2. **Bug Fixes**: MathJax rendering issues, TTS problems
3. **Performance**: Optimizations for loading and rendering
4. **Accessibility**: Improvements for students with disabilities
5. **Documentation**: Better guides and examples

## 📚 Question Content Guidelines

### Subject Coverage
Ensure questions cover:
- Core concepts
- Application problems
- Real-world scenarios
- Common misconceptions
- Past BECE exam topics

### Difficulty Levels
Mix question difficulty:
- **Easy (30%)**: Straightforward factual recall
- **Medium (50%)**: Requires application of concepts
- **Hard (20%)**: Requires analysis and synthesis

### Mathematical Notation Examples

```json
"question": "Solve: $2x + 5 = 13$"
"question": "Convert $0.000034$ to scientific notation"
"question": "What is $\\frac{3}{4} \\times \\frac{2}{5}$?"
"question": "If $y = x^2 + 3x - 2$, find $y$ when $x = 3$"
"question": "Calculate: $\\sqrt{144} + 2^3 - \\frac{10}{2}$"
```

### Formatting Best Practices
- Use **bold** for emphasis: `**important term**`
- Use `$LaTeX$` for math (inline) or `$$LaTeX$$` for block math
- Break long options with newlines for readability
- Use proper punctuation in explanations

## 🧪 Testing Your Contributions

Before submitting:

1. **Validate JSON**:
```javascript
JSON.parse(yourJsonString) // Should not throw error
```

2. **Check question completeness**:
   - All required fields present
   - Answer key matches an option
   - Explanation is detailed

3. **Test in app**:
   - Load questions successfully
   - Answers evaluate correctly
   - MathJax renders properly
   - TTS reads correctly

4. **Cross-browser testing**:
   - Chrome/Chromium
   - Firefox
   - Safari
   - Edge

## 📞 Questions About Contributing?

- **Open an issue** with your question
- **Email the maintainer**: Contact info in README.md
- **Check existing discussions** for similar questions

## 🎁 Recognition

Contributors will be:
- Listed in project contributors list
- Recognized in release notes for significant contributions
- Credited in documentation

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

## 🚀 Getting Help

- **Documentation**: See [README.md](README.md)
- **Issue Tracker**: Check existing issues and discussions
- **Developer Contact**: See README.md for contact information

---

**Thank you for making MYKHIL's BECE Study Guide better for students everywhere!** 🌟

**Happy Contributing! 🎓**
