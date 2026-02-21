# Contributing to Zebra Ecosystem

Thank you for your interest in contributing! This is primarily a personal project, but suggestions and improvements are welcome.

---

## Before You Contribute

### 1. Read the Security Architecture
☑️ Review [docs/SECURITY_ARCHITECTURE.md](docs/SECURITY_ARCHITECTURE.md)  
☑️ Understand the 3-zone security model  
☑️ Never include real credentials, IPs, or hostnames in commits  

### 2. Understand the Cost Framework
☑️ Review [COST_MANAGEMENT_STRATEGY.md](COST_MANAGEMENT_STRATEGY.md)  
☑️ Use cost-optimal AI models for contributions  
☑️ Consider using local Ollama for iteration  

### 3. Check the Model Registry
☑️ Review [AI_MODEL_REGISTRY_SYSTEM.md](AI_MODEL_REGISTRY_SYSTEM.md)  
☑️ Use appropriate models for different tasks  
☑️ Follow the decision matrix  

---

## Contribution Process

### 1. Fork and Clone

```bash
# Fork on GitHub, then:
git clone https://github.com/YOUR_USERNAME/zebra-ecosystem.git
cd zebra-ecosystem
git remote add upstream https://github.com/zebadee2kk/zebra-ecosystem.git
```

### 2. Create a Branch

```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix
```

### 3. Make Changes

☑️ Follow existing code style  
☑️ Add tests for new features  
☑️ Update documentation  
☑️ Run pre-commit hooks  

```bash
# Install pre-commit hooks
pre-commit install

# Run hooks manually
pre-commit run --all-files

# Run tests
make test

# Check code quality
make lint
```

### 4. Commit Your Changes

```bash
# Follow conventional commits format
git commit -m "feat: add new feature"
git commit -m "fix: resolve bug in module"
git commit -m "docs: update documentation"
git commit -m "chore: update dependencies"
```

### 5. Push and Create PR

```bash
git push origin feature/your-feature-name
```

Then create a Pull Request on GitHub.

---

## Code Style

### Python
- Use Black for formatting (`make format`)
- Use Ruff for linting (`make lint`)
- Follow PEP 8
- Type hints required for public APIs
- Docstrings for all public functions

### Commits
- Use conventional commits format
- Keep commits atomic (one logical change per commit)
- Write clear, descriptive commit messages

### Documentation
- Update README.md if changing user-facing features
- Update relevant docs/ files
- Add docstrings to new functions/classes

---

## Testing

### Required Tests
- Unit tests for new functions
- Integration tests for new features
- All tests must pass before PR

### Running Tests

```bash
# Run all tests
make test

# Run specific test file
pytest tests/zebra_core/test_config.py

# Run with coverage
make test-coverage
```

---

## Security Guidelines

### CRITICAL: Never Commit
❌ Real API keys or passwords  
❌ Real hostnames or IP addresses  
❌ Real database credentials  
❌ Personal or financial data  
❌ Cost tracking data (.cost_tracker.json)  

### Always Use Placeholders
✅ `[API_KEY]` instead of real keys  
✅ `[HOSTNAME]` instead of real hostnames  
✅ `[IP_ADDRESS]` instead of real IPs  
✅ Example data instead of real data  

### Before Committing

```bash
# Pre-commit hooks will run automatically
# They check for:
# - Secrets (gitleaks)
# - Credentials (detect-secrets)
# - Large files
# - Syntax errors

# Run manually:
pre-commit run --all-files
```

---

## AI-Assisted Development

### Model Selection for Contributions

| Task | Recommended Model |
|------|-------------------|
| Iteration / Debugging | Ollama Mistral (local, free) |
| Architecture / Design | Claude Sonnet |
| Code Review | Claude Sonnet or GPT-4 |
| Documentation | Claude Sonnet or Ollama |
| Research | Perplexity Free |

### Before Using Cloud AI

☑️ Check [templates/MODEL_SELECTION_CHECKLIST.md](templates/MODEL_SELECTION_CHECKLIST.md)  
☑️ Ensure no sensitive data in prompt  
☑️ Use placeholders for any real values  
☑️ Log usage if using paid API  

---

## Pull Request Guidelines

### PR Title Format
- Use conventional commits format
- Examples:
  - `feat: add cost tracking to homelab module`
  - `fix: resolve security check false positive`
  - `docs: update Phase 0 instructions`
  - `chore: update dependencies`

### PR Description Should Include
- What: Summary of changes
- Why: Motivation for changes
- How: Approach taken
- Tests: What tests were added/updated
- Security: Any security considerations
- Cost: Impact on AI model usage costs (if applicable)

### PR Checklist

```markdown
- [ ] Tests added/updated
- [ ] Documentation updated
- [ ] Pre-commit hooks pass
- [ ] All tests pass
- [ ] No secrets in commits
- [ ] Follows code style guidelines
- [ ] PR description complete
```

---

## Development Setup

### Initial Setup

```bash
# Clone repository
git clone https://github.com/zebadee2kk/zebra-ecosystem.git
cd zebra-ecosystem

# Create virtual environment
python3.11 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt

# Install pre-commit hooks
pre-commit install

# Set up environment
cp .env.example .env
# Edit .env with your values
```

### Daily Development

```bash
# Activate virtual environment
source venv/bin/activate

# Run tests before starting
make test

# Make your changes
# ...

# Run tests after changes
make test

# Check code quality
make lint

# Format code
make format

# Commit
git commit -m "feat: your feature"
```

---

## Questions or Issues?

- Open an issue: https://github.com/zebadee2kk/zebra-ecosystem/issues
- Check documentation: [DOCUMENTATION_INDEX.md](DOCUMENTATION_INDEX.md)
- Read the guides: [START_HERE.md](START_HERE.md)

---

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for contributing to Zebra Ecosystem!**

**Security-first. Cost-aware. AI-optimized.**