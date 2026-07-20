# Contributing to typedoc-plugin-not-exported

Thank you for your interest in contributing! This guide will help you get started.

## Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/typedoc-plugin-not-exported.git
   cd typedoc-plugin-not-exported
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```

## Development

### Build the project
```bash
npm run build
```

### Run tests
```bash
npm run test
```

This will:
- Generate documentation with `npm run test:gen`
- Run Jest tests with `npm run test:jest`
- Clean up with `npm run test:cleanup`

## Making Changes

1. **Create a feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** and ensure tests pass:
   ```bash
   npm run test
   ```

3. **Follow the code style**:
   - The project uses ESLint and Prettier
   - Run `npm run build` before committing

4. **Commit your changes** with clear messages:
   ```bash
   git commit -m "feat: add clear description of what changed"
   ```

5. **Push and create a Pull Request**:
   ```bash
   git push origin feature/your-feature-name
   ```

## Areas for Contribution

- 🐛 **Bug fixes** – Report or fix issues
- 📚 **Documentation** – Improve README or add examples
- ✨ **New features** – Suggest and implement enhancements
- 🧪 **Tests** – Increase test coverage
- 🔄 **Refactoring** – Improve code quality

## Questions?

- Open an [issue](https://github.com/protactiniumplatinumhyssop-cell/typedoc-plugin-not-exported/issues)
- Check existing issues for similar questions

## License

By contributing, you agree your contributions are licensed under CC0-1.0.

Thank you for helping make this plugin better! 🎉
