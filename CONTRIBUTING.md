# 🤝 Contributing to Cosmos E-commerce Platform

Thank you for your interest in contributing to Cosmos! We welcome contributions from everyone and are grateful for every pull request! 🎉

## 📋 Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Bug Reports](#bug-reports)
- [Feature Requests](#feature-requests)

## 📜 Code of Conduct

This project adheres to a code of conduct. By participating, you are expected to uphold this code. Please be respectful and inclusive in all interactions.

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/E-Cos-mos.git
   cd E-Cos-mos
   ```
3. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## 🔧 Development Setup

1. **Prerequisites**:
   - Java JDK 17 or higher
   - Maven 3.6+
   - Your favorite IDE (IntelliJ IDEA recommended)

2. **Build and run**:
   ```bash
   ./mvnw clean install
   ./mvnw spring-boot:run
   ```

3. **Verify setup**: Open http://localhost:8081 in your browser

## 🎯 How to Contribute

### 🐛 Bug Fixes
- Look for issues tagged with `bug`
- Provide clear reproduction steps
- Include screenshots if applicable
- Write tests for your fix

### ✨ New Features
- Check existing issues or create a new one for discussion
- Ensure the feature aligns with project goals
- Include comprehensive tests
- Update documentation as needed

### 📚 Documentation
- Improve README, code comments, or JavaDoc
- Add examples and usage guides
- Fix typos and grammar

### 🎨 UI/UX Improvements
- Ensure responsive design
- Follow the existing design system
- Test on multiple browsers and devices
- Include before/after screenshots

## 🔄 Pull Request Process

1. **Update your fork**:
   ```bash
   git checkout master
   git pull upstream master
   git checkout your-feature-branch
   git rebase master
   ```

2. **Test your changes**:
   ```bash
   ./mvnw test
   ./mvnw spring-boot:run
   ```

3. **Commit your changes**:
   ```bash
   git add .
   git commit -m "feat: add amazing new feature"
   ```

4. **Push to your fork**:
   ```bash
   git push origin your-feature-branch
   ```

5. **Create a Pull Request** on GitHub with:
   - Clear title and description
   - Reference any related issues
   - Screenshots for UI changes
   - List of changes made

## 🎨 Coding Standards

### Java Code
- Follow [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- Use meaningful variable and method names
- Add JavaDoc comments for public methods
- Keep methods focused and concise

### HTML/CSS
- Use semantic HTML5 elements
- Follow BEM naming convention for CSS classes
- Ensure responsive design (mobile-first approach)
- Maintain consistent indentation (2 spaces)

### Thymeleaf Templates
- Use proper Thymeleaf syntax and security features
- Escape user input appropriately
- Follow consistent template structure

### Commit Messages
Use [Conventional Commits](https://www.conventionalcommits.org/):
- `feat:` for new features
- `fix:` for bug fixes
- `docs:` for documentation
- `style:` for formatting changes
- `refactor:` for code refactoring
- `test:` for adding tests
- `chore:` for maintenance tasks

Examples:
```
feat: add product rating system
fix: resolve cart total calculation bug
docs: update API documentation
style: improve product card styling
```

## 🐛 Bug Reports

When filing a bug report, please include:

1. **Bug Description**: Clear and concise description
2. **Steps to Reproduce**: Numbered steps to reproduce the issue
3. **Expected Behavior**: What you expected to happen
4. **Actual Behavior**: What actually happened
5. **Screenshots**: If applicable
6. **Environment**:
   - OS and version
   - Java version
   - Browser and version
   - Application version

## 💡 Feature Requests

For feature requests, please provide:

1. **Feature Description**: Clear description of the feature
2. **Use Case**: Why this feature would be useful
3. **Acceptance Criteria**: How we know the feature is complete
4. **Mockups/Examples**: Visual examples if applicable

## 🏷️ Issue Labels

We use these labels to organize issues:

- 🐛 `bug` - Something isn't working
- ✨ `enhancement` - New feature or request
- 📚 `documentation` - Improvements or additions to docs
- 🎨 `design` - Design-related issues
- 🚀 `performance` - Performance improvements
- 🔒 `security` - Security-related issues
- 🧪 `testing` - Testing improvements
- 🏁 `good first issue` - Good for newcomers

## 🎉 Recognition

Contributors are recognized in:
- README.md contributors section
- Release notes
- Special mentions in commits

## 📞 Getting Help

Need help with contributing? Reach out to us:

- 💬 [GitHub Discussions](https://github.com/nishu-kumari14/E-Cos-mos/discussions)
- 📧 Email: nishukumari14@example.com
- 🐛 [GitHub Issues](https://github.com/nishu-kumari14/E-Cos-mos/issues)

## 🙏 Thank You!

Every contribution, no matter how small, makes a difference. Thank you for helping make Cosmos better! 

---

<div align="center">

**Happy Contributing! 🚀**

Made with ❤️ by the Cosmos community

</div>
