# Contributing to Ultimate REMIX 🎮

Thank you for your interest in contributing to Ultimate REMIX! This document provides guidelines and information for contributors.

## 🤝 Code of Conduct

We are committed to providing a welcoming and inspiring community for all. Please be respectful and constructive in all interactions.

## 🚀 How to Contribute

### 🐛 Reporting Bugs

Before submitting a bug report:
1. Check the [Issues page](https://github.com/prathamamritkar/ultimate-remix/issues) to see if it's already reported
2. Try to reproduce the bug with the latest version
3. Gather relevant information about your environment

When submitting a bug report, include:
- **Browser and version** (e.g., Chrome 96.0.4664.110)
- **Operating System** (e.g., Windows 10, macOS 12.1, Android 11)
- **Device type** (Desktop, Mobile, Tablet)
- **Steps to reproduce** the issue
- **Expected behavior** vs **actual behavior**
- **Screenshots or videos** if applicable
- **Console errors** (press F12 → Console tab)

### 💡 Suggesting Features

We welcome feature suggestions! Before submitting:
1. Check existing issues to avoid duplicates
2. Consider if the feature fits the game's core design
3. Think about implementation complexity

Include in your feature request:
- **Clear description** of the proposed feature
- **Use case scenarios** - when/why would this be useful?
- **Possible implementation approach** (if you have ideas)
- **Alternative solutions** you've considered

### 🔧 Code Contributions

#### Getting Started
1. Fork the repository
2. Create a new branch from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes
4. Test thoroughly on multiple browsers/devices
5. Submit a pull request

#### Development Setup
```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/ultimate-remix.git
cd ultimate-remix

# Start a local server for testing
python -m http.server 8000
# OR
npx http-server

# Open http://localhost:8000 in your browser
```

#### Code Style Guidelines

**JavaScript:**
- Use ES6+ features where appropriate
- Prefer `const` and `let` over `var`
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions focused and small
- Use consistent indentation (2 spaces)

**HTML/CSS:**
- Use semantic HTML elements
- Maintain responsive design principles
- Keep CSS organized and commented
- Test on multiple screen sizes

**Game-Specific:**
- Maintain 60 FPS performance
- Consider mobile device limitations
- Preserve existing game balance
- Test across different skill levels

#### Testing Your Changes
Before submitting, please test:
- **Functionality**: Does your feature work as intended?
- **Performance**: No significant FPS drops or memory leaks?
- **Compatibility**: Works on Chrome, Firefox, Safari, Edge?
- **Mobile**: Responsive and touch-friendly?
- **Accessibility**: Keyboard navigation and screen reader friendly?

### 📝 Pull Request Process

1. **Update documentation** if you're changing functionality
2. **Add tests** if applicable (or describe manual testing done)
3. **Update CHANGELOG.md** if it's a notable change
4. **Ensure clean commit history** - squash commits if needed
5. **Write clear PR description** explaining your changes

#### Pull Request Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Performance improvement
- [ ] Documentation update
- [ ] Other (specify)

## Testing Done
- [ ] Tested on Chrome/Firefox/Safari/Edge
- [ ] Tested on mobile devices
- [ ] Tested game mechanics
- [ ] Performance testing

## Screenshots (if applicable)
Add screenshots showing your changes

## Additional Notes
Any additional context or considerations
```

## 🎮 Game Design Guidelines

### Core Principles
- **Accessibility First**: Everyone should be able to play
- **Progressive Difficulty**: Gentle learning curve
- **Educational Value**: Learning through play
- **Performance**: Smooth 60 FPS experience
- **Mobile-Friendly**: Touch controls and responsive design

### Adding New Features
Consider these questions:
- Does it enhance the core gameplay loop?
- Is it accessible to players of all skill levels?
- Does it maintain the educational aspects?
- Can it be implemented efficiently?
- Is it consistent with existing UI/UX patterns?

### Content Guidelines
- Keep content family-friendly
- Ensure educational accuracy
- Consider internationalization
- Maintain positive, encouraging tone

## 🏗️ Technical Architecture

### File Organization
```
index.html              # Single-file game architecture
├── Game States         # Loading, Playing, Game Over, etc.
├── World Systems       # 5 different game worlds
├── Player Progression  # XP, levels, equipment
├── Card System         # Collectible power-ups
├── Audio System        # Sound effects and music
├── Input Handling      # Mouse, touch, keyboard
└── Rendering Engine    # Canvas 2D graphics
```

### Performance Considerations
- Game loop runs at 60 FPS target
- Canvas operations are batched
- Object pooling for frequently created/destroyed objects
- Efficient collision detection algorithms
- Memory-conscious asset loading

## 🌍 Internationalization

If contributing translations or text content:
- Use clear, simple language
- Consider cultural context
- Test text layout with longer translations
- Maintain consistent terminology

## 📚 Resources

### Learning Resources
- [MDN Web Docs - Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [MDN Web Docs - Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [HTML5 Game Development](https://developer.mozilla.org/en-US/docs/Games)

### Tools
- Browser Developer Tools for debugging
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) for performance auditing
- [Can I Use](https://caniuse.com/) for browser compatibility

## ❓ Questions?

If you have questions about contributing:
1. Check existing [Issues](https://github.com/prathamamritkar/ultimate-remix/issues)
2. Create a new issue with the "question" label
3. Join discussions in existing pull requests

## 🙏 Recognition

Contributors will be acknowledged in:
- README.md contributors section
- Git commit history
- Special thanks in game credits (for significant contributions)

Thank you for helping make Ultimate REMIX better! 🎮✨