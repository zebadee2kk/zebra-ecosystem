# Quick Start Guide
## Get Up and Running in 15 Minutes

---

## Prerequisites

☑️ Python 3.11+  
☑️ Git  
☑️ Claude Pro account OR Ollama running locally  
☑️ 1Password or password manager  

---

## Step 1: Clone & Setup (5 minutes)

```bash
# Clone the repository
git clone https://github.com/zebadee2kk/zebra-ecosystem.git
cd zebra-ecosystem

# Create virtual environment
python3.11 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies (when available)
pip install -r requirements.txt  # Create this in Phase 1
```

---

## Step 2: Environment Setup (5 minutes)

```bash
# Copy environment template
cp .env.example .env

# Edit .env with your actual credentials
# Use placeholders for now if you don't have all credentials
nano .env  # or vim, or your preferred editor

# CRITICAL: Never commit .env!
git status  # Verify .env is NOT in git (should be ignored)
```

---

## Step 3: Verify Setup (5 minutes)

```bash
# Check Python version
python --version
# Should be 3.11 or higher

# Verify git is clean
git status
# Should show only untracked files (not .env)

# Check if Ollama is available (optional)
curl http://localhost:11434/api/version
# Or if on remote VM:
curl http://[OLLAMA_VM_IP]:11434/api/version
```

---

## Step 4: Read Documentation (Ongoing)

### Today (15 minutes)
1. ☑️ [README.md](README.md) - Project overview
2. ☑️ [START_HERE.md](START_HERE.md) - Executive summary
3. ☑️ [COMPLETE_PROJECT_SUMMARY.md](COMPLETE_PROJECT_SUMMARY.md) - Systems overview

### Before Phase 0 (30 minutes)
4. Retrieve large docs from Perplexity conversation:
   - COST_MANAGEMENT_STRATEGY.md
   - AI_MODEL_REGISTRY_SYSTEM.md
   - PHASE_0_EXTENDED_WITH_MODELS.md
   - ZEBRA_COMPLETE_BRIEF.md

### During Phase 0 (3 hours)
5. Follow **PHASE_0_EXTENDED_WITH_MODELS.md** step-by-step

---

## Step 5: Start Phase 0 (When Ready)

```bash
# Phase 0 consists of three parts:
# Part A: Security foundation (1 hour)
# Part B: Cost management foundation (1 hour)  
# Part C: Model registry foundation (1 hour)

# Follow PHASE_0_EXTENDED_WITH_MODELS.md for details
```

---

## What You Have Now

✅ Repository cloned  
✅ Virtual environment created  
✅ .env configured (with placeholders)  
✅ Documentation read  
☑️ Ready to start Phase 0  

---

## Next Steps

### Immediate (Today)
1. Retrieve the 4 large documentation files from your Perplexity conversation
2. Add them to the repository root
3. Read PHASE_0_EXTENDED_WITH_MODELS.md
4. Start Phase 0 Part A (Security)

### This Week (Days 1-3)
1. Complete Phase 0 (all three parts)
2. Start Phase 1 (Scaffold)
3. Set up testing framework

### This Month (Days 4-10)
1. Complete Phases 2-5
2. Build zebra_core, domains, and apps
3. Full test coverage
4. Production-ready ecosystem

---

## Troubleshooting

### Python version too old
```bash
# Install Python 3.11+ using pyenv
curl https://pyenv.run | bash
pyenv install 3.11.7
pyenv global 3.11.7
```

### .env in git
```bash
# If you accidentally added .env to git:
git rm --cached .env
git commit -m "Remove .env from git"
# Verify .gitignore includes .env
cat .gitignore | grep .env
```

### Ollama not accessible
```bash
# If Ollama is on a different machine:
# 1. Update OLLAMA_HOST in .env
# 2. Ensure firewall allows port 11434
# 3. Test: curl http://[OLLAMA_VM_IP]:11434/api/version
```

---

## Key Commands (After Phase 1)

```bash
# Run tests
make test

# Check code quality
make lint

# Format code  
make format

# Security check
make security-check

# Cost reports
make cost-weekly
make cost-monthly

# Model registry
make model-registry
make model-check
make model-report
```

---

## Getting Help

### Documentation
- [DOCUMENTATION_INDEX.md](DOCUMENTATION_INDEX.md) - Guide to all docs
- [README.md](README.md) - Project overview
- [START_HERE.md](START_HERE.md) - Where to begin

### Issues
- GitHub Issues: https://github.com/zebadee2kk/zebra-ecosystem/issues

---

**You're ready! Start with Phase 0 when you have 3 hours.**

**Follow PHASE_0_EXTENDED_WITH_MODELS.md for the complete setup.**

**Build once. Reuse forever.**