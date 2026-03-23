---
name: compliance-assessment-tools
description: Browser-based interactive compliance assessment wizards for EU AI Act and related frameworks
version: 0.1.0
---

# Compliance Assessment Tools Skill

Use this skill when the user needs interactive browser-based tools for conducting AI compliance assessments.

## When to use
- User wants to assess their AI system against the EU AI Act
- User needs interactive compliance checklists or risk assessments
- User mentions "compliance wizard", "risk assessment tool", or "EU AI Act assessment"

## How to use

Open `index.html` in a browser to access the launcher, which provides links to all 23 assessment tools.

### Available tools include:
- Risk Classification Wizard — Determine EU AI Act risk tier
- FRIA (Fundamental Rights Impact Assessment)
- Technical Documentation Generator
- Data Governance Assessment
- Transparency Requirements Checklist
- Human Oversight Evaluation
- Conformity Assessment Planner
- And 16 more specialized assessment tools

## Key behaviors
- All tools run entirely in the browser (no server required)
- Built on the zero-dep-wizard framework (createWizard pattern)
- State auto-persists to sessionStorage (survives page reloads)
- Consistent navy/amber/teal design system
- Each tool outputs structured assessment results that can be exported
