# 🦓 Zebra Ecosystem

> **AI-Powered Python Ecosystem with Integrated Security, Cost Control, and Model Intelligence**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

---

## 📋 What Is This?

A **production-ready Python monorepo** that solves three critical problems for AI-assisted development:

1. **🔒 Security**: 3-zone model ensures sensitive data never leaks to cloud AI
2. **💰 Cost Control**: Automatic tracking prevents expensive token waste
3. **🧠 Model Intelligence**: Living registry optimizes AI model selection

**Built for**: Homelab automation, trading systems, AI agents, and personal productivity tools.

---

## 🚀 Quick Start

### Prerequisites
- Python 3.11+
- Git
- Ollama (for local AI) or Claude Pro subscription
- 1Password or similar password manager

### Installation

```bash
# Clone the repository
git clone https://github.com/zebadee2kk/zebra-ecosystem.git
cd zebra-ecosystem

# Set up the environment
make setup

# Run tests
make test

# See available models
make model-registry

# Check cost tracking
make cost-weekly
```

---

## 📚 Documentation

### Start Here
1. **[START_HERE.md](START_HERE.md)** - Executive summary and 10-day timeline
2. **[COMPLETE_PROJECT_SUMMARY.md](COMPLETE_PROJECT_SUMMARY.md)** - Overview of all systems
3. **[PHASE_0_EXTENDED_WITH_MODELS.md](PHASE_0_EXTENDED_WITH_MODELS.md)** - Today's action items

### Core Frameworks
- **Security**: [SECURITY_ARCHITECTURE.md](docs/SECURITY_ARCHITECTURE.md)
- **Cost Control**: [COST_MANAGEMENT_STRATEGY.md](COST_MANAGEMENT_STRATEGY.md)
- **Model Intelligence**: [AI_MODEL_REGISTRY_SYSTEM.md](AI_MODEL_REGISTRY_SYSTEM.md)

### Architecture
- **[ZEBRA_COMPLETE_BRIEF.md](ZEBRA_COMPLETE_BRIEF.md)** - Master architecture reference
- **[ACTION_PLAN_UPDATED_WITH_COSTS.md](ACTION_PLAN_UPDATED_WITH_COSTS.md)** - Execution plan

---

## 🏗️ Architecture

```
zebra-ecosystem/
├── src/zebra_core/          # Shared building blocks
│   ├── cost/                # Cost tracking
│   ├── models/              # Model registry
│   ├── config/              # Configuration management
│   └── logging/             # Structured logging
├── src/domains/             # Business logic modules
│   ├── homelab/             # Proxmox, networking, monitoring
│   ├── agents/              # AI agents and workflows
│   ├── trading/             # Trading systems
│   └── personal/            # Personal productivity
├── apps/                    # CLI applications
│   ├── homelab_assistant/   # Homelab management CLI
│   └── whoami_ai/           # AI conversation collator
├── docs/                    # Documentation
├── templates/               # Decision templates
└── infra/                   # Infrastructure and tooling
```

### The Three Layers

1. **zebra_core**: Reusable building blocks (config, logging, CLI framework)
2. **domains**: Business logic modules (homelab, trading, agents, personal)
3. **apps**: Thin CLI wrappers that compose domain functionality

---

## 🔒 Security Model

### 3-Zone Architecture

| Zone | Location | Can Handle | Use For |
|------|----------|------------|----------|
| **Zone 1** | Cloud AI | Placeholders only | Architecture, design, generic code |
| **Zone 2** | Local Ollama | Real data | Sensitive analysis, financial data |
| **Zone 3** | Air-gapped | Everything | Maximum security requirements |

**Before every cloud AI prompt**: Use our [safety checklist](templates/AI_SAFETY_AND_COST_CHECKLIST.md)

---

## 💰 Cost Control

### Optimal Setup: $20-30/month

| Tool | Cost | Usage |
|------|------|-------|
| Ollama (local) | FREE | 60% of work (iteration, debugging) |
| Claude Pro | $20/mo | 30% of work (architecture, review) |
| Perplexity Free | FREE | Research, web search |
| GitHub Copilot | $0-10/mo | Inline code completion |

### Cost Tracking

```bash
# Weekly spend report
make cost-weekly

# Monthly analysis
make cost-monthly

# Model usage patterns
make model-report
```

---

## 🧠 Model Intelligence

### 7 AI Models Cataloged

- **Claude Opus**: Best reasoning (10/10), expensive
- **Claude Sonnet**: Best value (9/10 reasoning, 8/10 speed)
- **Claude Haiku**: Fastest (10/10 speed), cheap
- **Ollama Mistral**: Local, FREE, good for iteration
- **Ollama Llama2**: Local, FREE, stable baseline
- **GPT-4 Turbo**: Second opinions
- **Perplexity**: Research with web search

### Decision Matrix

```bash
# See which model for which task
cat docs/MODEL_DECISION_MATRIX.md

# View all available models
make model-registry

# Check for new models
make model-check
```

---

## 🛠️ Development

### Daily Workflow

```bash
# Before asking any AI:
# 1. Check: templates/MODEL_SELECTION_CHECKLIST.md
# 2. Pick model: docs/MODEL_DECISION_MATRIX.md
# 3. Use placeholders for sensitive data
# 4. Ask question
# 5. Log usage

# Run tests
make test

# Lint code
make lint

# Format code
make format

# Security check
make security-check
```

### Weekly Reviews

```bash
# Every Friday
make cost-weekly      # Spending trends
make model-report     # Decision patterns
make model-check      # New models available
```

---

## 📦 Current Status

### Phase 0: Foundation ✅
- [x] Security framework (3-zone model)
- [x] Cost tracking system
- [x] Model registry (7 models)
- [x] Pre-commit hooks
- [x] Documentation

### Phase 1: Scaffold (In Progress)
- [ ] Directory structure
- [ ] Core modules
- [ ] Testing framework
- [ ] CI/CD pipeline

### Phase 2-5: Development (Planned)
- [ ] zebra_core building blocks
- [ ] Domain modules (homelab, agents, trading, personal)
- [ ] CLI applications
- [ ] Full test coverage

---

## 🤝 Contributing

This is a personal project, but suggestions and issues are welcome!

1. Check [SECURITY_ARCHITECTURE.md](docs/SECURITY_ARCHITECTURE.md) before contributing
2. Use [MODEL_SELECTION_CHECKLIST.md](templates/MODEL_SELECTION_CHECKLIST.md) for AI assistance
3. Follow the pre-commit hooks (automatically enforced)

---

## 📄 License

MIT License - See [LICENSE](LICENSE) for details

---

## 🙏 Acknowledgments

- **Anthropic Claude** - AI architecture and development assistance
- **Ollama** - Local AI inference
- **Proxmox Community** - Homelab inspiration

---

## 📞 Contact

**RicheeRich** - London-based, 25 years IT/cybersec industry

- GitHub: [@zebadee2kk](https://github.com/zebadee2kk)
- Location: London

---

**Built with AI assistance. Secured by design. Optimized for cost.**

*Start with [START_HERE.md](START_HERE.md) → Follow [PHASE_0_EXTENDED_WITH_MODELS.md](PHASE_0_EXTENDED_WITH_MODELS.md) → Build in 10 days*