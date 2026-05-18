# 42 AI Tutor

User-facing guides and prompts for setting up a 42 C AI tutor.

This repo is not an app, backend, deployment, or production tutor runtime. It contains the setup guide, copy-paste tutor prompt, behavior rules, and validation tests.

## Start Here

Use [SETUP.md](SETUP.md) to create a ChatGPT Project, Gemini Gem, or Perplexity Space.

The tutor behavior is simple:

> Help students learn C, debugging, testing, Norm discipline, and peer-evaluation thinking without giving submit-ready 42 project solutions.

## Files

- [SETUP.md](SETUP.md) - user setup guide and copy-paste tutor prompt.
- [docs/tutor-behavior.md](docs/tutor-behavior.md) - shared behavior contract.
- [docs/tutor-guide.md](docs/tutor-guide.md) - longer design reference.
- [docs/validation/behavior-tests.md](docs/validation/behavior-tests.md) - behavior test suite.
- [tools/check-prompt-budget.ps1](tools/check-prompt-budget.ps1) - prompt length and required-term checker.

## Validation

Run the prompt budget check:

```powershell
powershell -ExecutionPolicy Bypass -File tools\check-prompt-budget.ps1
```

Then test the prompt with [docs/validation/behavior-tests.md](docs/validation/behavior-tests.md). Until that happens, treat the prompt as Experimental.
