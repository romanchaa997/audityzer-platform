# Contributing to Audityzer Platform

🎉 **Thank you for your interest in contributing to Audityzer!**

We welcome contributions from the community to help make Web3 security accessible and effective for everyone.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Commit Messages](#commit-messages)
- [Issue Labels](#issue-labels)

## 📜 Code of Conduct

This project adheres to the Contributor Covenant [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## 🤝 How Can I Contribute?

### Reporting Bugs

- Check if the bug has already been reported in [Issues](https://github.com/romanchaa997/audityzer-platform/issues)
- Use the bug report template
- Include detailed reproduction steps
- Attach logs and screenshots if applicable

### Suggesting Enhancements

- Use the feature request template
- Explain the problem you're trying to solve
- Provide examples of how the feature would work

### Code Contributions

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Make your changes**
4. **Test thoroughly**
5. **Commit** (`git commit -m 'Add AmazingFeature'`)
6. **Push** (`git push origin feature/AmazingFeature`)
7. **Open a Pull Request**

## 🛠️ Development Setup

### Prerequisites

- Node.js >= 18.0.0
- npm >= 9.0.0
- Git

### Installation

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/audityzer-platform.git
cd audityzer-platform

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Run development server
npm run dev
```

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run with coverage
npm test -- --coverage
```

### Linting

```bash
# Check for linting errors
npm run lint

# Auto-fix linting errors
npm run lint:fix
```

## 🔄 Pull Request Process

### Before Submitting

- [ ] Code follows the project's coding standards
- [ ] All tests pass (`npm test`)
- [ ] No linting errors (`npm run lint`)
- [ ] Documentation is updated if needed
- [ ] Commit messages follow the convention
- [ ] PR description clearly describes the changes

### PR Title Format

```
<type>(<scope>): <short summary>
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

**Examples:**
- `feat(audit): add support for Polygon network`
- `fix(scanner): resolve XSS detection false positives`
- `docs(readme): update installation instructions`

### Review Process

1. At least one maintainer must review your PR
2. All CI checks must pass
3. Address any requested changes
4. Once approved, a maintainer will merge your PR

## 💻 Coding Standards

### JavaScript/Node.js

- Follow [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- Use ES6+ features
- Prefer `const` over `let`, avoid `var`
- Use meaningful variable names
- Add JSDoc comments for functions

```javascript
/**
 * Analyzes a smart contract for vulnerabilities
 * @param {string} contractAddress - Ethereum contract address
 * @param {Object} options - Analysis options
 * @returns {Promise<Object>} Analysis results
 */
async function analyzeContract(contractAddress, options) {
  // Implementation
}
```

### File Structure

```
src/
├── api/           # API routes
├── controllers/   # Business logic
├── models/        # Data models
├── services/      # External services
├── utils/         # Utility functions
├── config/        # Configuration
└── tests/         # Test files
```

### Testing

- Write tests for new features
- Maintain test coverage above 80%
- Use descriptive test names

```javascript
describe('Smart Contract Analyzer', () => {
  it('should detect reentrancy vulnerability', async () => {
    // Test implementation
  });
});
```

## 📝 Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

**Good examples:**
```
feat(api): add endpoint for batch contract analysis

Implements batch processing for multiple contracts
to improve performance and reduce API calls.

Closes #123
```

```
fix(scanner): resolve false positive in gas optimization

The analyzer was incorrectly flagging optimized loops.
Updated detection logic to check for specific patterns.
```

## 🏷️ Issue Labels

- `bug` - Something isn't working
- `enhancement` - New feature or request
- `documentation` - Improvements to docs
- `good first issue` - Good for newcomers
- `help wanted` - Extra attention needed
- `security` - Security-related issue
- `performance` - Performance improvement
- `question` - Further information requested

## 🔒 Security

If you discover a security vulnerability, **DO NOT** open a public issue.

Instead, email us at: **rigoryanych1397@gmail.com**

See [SECURITY.md](SECURITY.md) for more details.

## 🌟 Recognition

All contributors will be recognized in our:
- README.md Contributors section
- Release notes
- Monthly contributor spotlight

## 📞 Questions?

Feel free to:
- Open a [Discussion](https://github.com/romanchaa997/audityzer-platform/discussions)
- Join our community chat (coming soon)
- Email: rigoryanych1397@gmail.com

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for making Audityzer better! 🚀**
