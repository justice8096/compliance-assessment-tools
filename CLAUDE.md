# Compliance Assessment Tools

## Purpose
Bundle of 21 browser-based interactive wizard tools for AI compliance assessment. Each tool uses the createWizard() framework with sessionStorage persistence, zero external dependencies.

## Tools & Stack
- **Vanilla JavaScript** (no framework)
- **createWizard()** from shared.js
- Zero external dependencies

## Directory Structure
```
index.html               — Launcher page listing all 21 tools
tools/
  shared.js              — Wizard framework and UI primitives
  risk-classification.html
  bias-testing.html
  consent-design.html
  human-oversight.html
  impact-risk-scoring.html
  security-assessment.html
  llm-selector.html
  supply-chain-risk.html
  ... (21 tools total)
```

## Running
```bash
npx serve .
# Open http://localhost:3000
```

## Assessment Categories
- **Risk & Impact** (4): Risk Classification, Impact Scoring, PIA Assessment, Supply Chain Risk
- **Privacy** (4): Consent Design, Consent Records Audit, DSR Rights, Training Data Disclosure
- **Disclosure** (4): Disclosure Toolkit, Content Labeling, Transparency Documentation, Content Moderation
- **Systems** (3): Automated Decision Logic, Human Oversight, LLM Selector
- **Governance** (3): Governance Framework, Incident Management, Conformity Assessment
- **Training** (3): AI Literacy Training, Bias Testing, Security Assessment

## Technical Notes
- All tools use sessionStorage for state persistence (survives page reloads)
- Each tool has stateKey, getState, setState for auto-persist
- Design: navy #0B1426, amber #D4943A, teal #2A7B7B
- Zero innerHTML — all DOM manipulation via createElement/textContent
- Export to markdown and JSON config formats
