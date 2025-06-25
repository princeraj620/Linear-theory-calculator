# Contributing to Linear Theory Calculator

Thank you for your interest in contributing to the Linear Theory Calculator! This document provides guidelines and information for contributors.

## 🤝 How to Contribute

### Reporting Bugs

1. Check if the bug has already been reported in the [Issues](https://github.com/princeraj620/linear-theory-calculator/issues) section
2. If not, create a new issue with:
   - A clear and descriptive title
   - Steps to reproduce the bug
   - Expected vs actual behavior
   - Browser and OS information
   - Screenshots if applicable

### Suggesting Enhancements

1. Check if the enhancement has already been suggested
2. Create a new issue with:
   - A clear and descriptive title
   - Detailed description of the proposed feature
   - Use cases and benefits
   - Mockups or examples if applicable

### Code Contributions

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
   - Follow the coding standards below
   - Add tests if applicable
   - Update documentation as needed
4. **Commit your changes**
   ```bash
   git commit -m "Add: brief description of changes"
   ```
5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```
6. **Create a Pull Request**
   - Provide a clear description of changes
   - Reference any related issues
   - Include screenshots for UI changes

## 📋 Coding Standards

### HTML
- Use semantic HTML5 elements
- Maintain proper indentation (2 spaces)
- Include proper meta tags
- Ensure accessibility (ARIA labels, alt text)

### CSS
- Use consistent naming conventions
- Prefer CSS Grid and Flexbox for layouts
- Use CSS custom properties for theming
- Ensure responsive design
- Follow BEM methodology when possible

### JavaScript
- Use ES6+ features
- Maintain consistent indentation (2 spaces)
- Add comments for complex logic
- Use meaningful variable and function names
- Handle errors gracefully

### General
- Keep functions small and focused
- Write self-documenting code
- Test your changes thoroughly
- Ensure cross-browser compatibility

## 🧪 Testing

Before submitting your contribution:

1. **Test in multiple browsers** (Chrome, Firefox, Safari, Edge)
2. **Test on mobile devices** or use browser dev tools
3. **Validate HTML** using W3C validator
4. **Check for JavaScript errors** in browser console
5. **Test all functionality** including edge cases

## 📚 Documentation

When adding new features:

1. Update the README.md if needed
2. Add inline comments for complex algorithms
3. Update any relevant documentation files
4. Include usage examples

## 🎯 Project Structure

```
linear-theory-calculator/
├── linear theory algorithm.html    # Main application
├── index.html                      # Entry point
├── README.md                       # Project documentation
├── CONTRIBUTING.md                 # This file
├── LICENSE                         # MIT License
├── package.json                    # Project metadata
└── .gitignore                      # Git ignore rules
```

## 🚀 Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/princeraj620/linear-theory-calculator.git
   cd linear-theory-calculator
   ```

2. **Start local server**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. **Open in browser**
   - Navigate to `http://localhost:8000`
   - Or open `linear theory algorithm.html` directly

## 📝 Commit Message Guidelines

Use conventional commit format:

- `Add:` for new features
- `Fix:` for bug fixes
- `Update:` for improvements
- `Refactor:` for code refactoring
- `Docs:` for documentation changes
- `Style:` for formatting changes

Example:
```
Add: export results to CSV functionality
Fix: calculation error in fan parameters
Update: improve responsive design for mobile
```

## 🔍 Review Process

1. All contributions will be reviewed
2. Maintainers may request changes
3. Once approved, your PR will be merged
4. Contributors will be added to the contributors list

## 📞 Getting Help

If you need help:

1. Check existing issues and discussions
2. Create a new issue with your question
3. Tag it appropriately (question, help-wanted, etc.)

## 🙏 Recognition

Contributors will be:

- Listed in the README.md
- Added to the contributors section
- Recognized in release notes

## 📄 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing to the Linear Theory Calculator! 🎉 