# Interactive Assessment Tools Bundle

21 interactive web-based tools for comprehensive AI compliance assessment. Works offline, no backend required.

## Overview

This bundle provides interactive guided assessments across all compliance domains. Each tool features:

- **Wizard Framework** — Step-by-step guided workflows
- **Decision Trees** — Logic-driven question flows
- **Scoring Engines** — Automated risk/readiness scoring
- **Export Capability** — Download results as JSON/markdown
- **Responsive Design** — Works on desktop, tablet, mobile

## The 21 Tools

### Risk & Impact Assessment (4)

1. **Impact & Risk Scoring** — Assess AI system impact across multiple dimensions (performance, fairness, security, privacy, safety)
2. **Risk Classification** — Classify systems by regulatory risk tier per AI Act and equivalent regulations
3. **Privacy Impact Assessment** — Comprehensive PIA for data processing in AI systems
4. **Conformity Assessment** — Full conformity checklist against regulatory requirements

### Privacy & Consent (4)

5. **Consent Design Wizard** — Design user-facing consent flows for transparency and autonomy
6. **Consent Records Audit** — Validate consent documentation and storage practices
7. **Data Subject Rights Implementation** — Plan and execute DSR implementation (access, deletion, portability, objection)
8. **Privacy Impact Assessment** — Multi-jurisdiction privacy impact assessment

### Disclosure & Transparency (4)

9. **Disclosure Toolkit** — Generate AI system disclosure materials for end users
10. **Content Labeling Strategy** — Framework for labeling AI-generated and synthetic content
11. **Training Data Disclosure** — Document training data sources, composition, bias assessment
12. **Transparency Documentation** — Create detailed system functionality and limitation docs

### Systems & Operations (3)

13. **Automated Decision Logic** — Evaluate automated decision systems for bias, transparency, oversight
14. **Content Moderation Assessment** — Evaluate moderation systems for fairness and appeal mechanisms
15. **Human Oversight Design** — Design meaningful human oversight in automated decisions

### Risk Management (3)

16. **Incident Management Planning** — Prepare incident response procedures for AI failures
17. **Supply Chain Risk Management** — Identify third-party risks and vendor compliance
18. **Security Assessment** — Evaluate AI system security posture and threat landscape

### Governance & Support (3)

19. **Governance Framework** — Build governance structures with oversight, roles, accountability
20. **AI Literacy Training** — Assess organizational AI knowledge and training needs
21. **LLM Model Selector** — Compare LLMs across compliance, capability, cost, safety

## Quick Start

```bash
# Setup
npm install
npm run serve

# Open browser
http://localhost:3000
```

Then click any tool to launch the interactive wizard.

## Using the Tools

### Workflow Example: Bias Testing

1. **Open Tool** — Click "Bias Testing Framework"
2. **Answer Questions** — Respond to guided questions about your system
3. **Review Scoring** — See real-time risk and readiness scores
4. **Export Results** — Download as JSON or markdown
5. **Integrate** — Import findings into compliance documentation

### Data Privacy

All data stays in your browser. No information is sent to servers.

## Tool Features

### Question Types

- **Multiple Choice** — Select from predefined options
- **Text Input** — Free-form responses with validation
- **Numerical** — Percentages, counts, dates
- **File Upload** — Attach supporting documentation
- **Wizard Branching** — Questions adapt based on previous answers

### Output Formats

- **JSON Export** — Raw structured data for integration
- **Markdown Report** — Formatted report for documentation
- **PDF** — Print-friendly compliance evidence
- **CSV** — Spreadsheet for cross-tool analysis

### Scoring Systems

Each tool includes proprietary scoring:

- **Readiness Score** (0-100) — Organizational readiness
- **Risk Score** (0-100) — Compliance risk level
- **Coverage Percentage** — Completeness of implementation
- **Action Items** — Prioritized remediation list

## Wizard Framework

The shared wizard framework provides:

- **Progress Tracking** — See completion status
- **Save/Resume** — Continue tools later
- **Autosave** — Local browser storage
- **Validation** — Catch required fields
- **Branching Logic** — Skip irrelevant questions
- **Context Help** — Inline guidance for complex topics

## Integration

### With Other Tools

Use results from assessment tools in:

- Compliance-autofill (pre-populate template fields)
- AI Regulatory Knowledge Base (reference applicable laws)
- Compliance Deadline Tracker (set review dates)

### With Documentation

Export tool results to markdown for inclusion in:

- Compliance documentation
- Risk registers
- Evidence portfolios
- Board presentations

## Customization

Edit `index.html` to customize:

```javascript
// Add your own tools
const tools = [
  {
    name: "Custom Tool Name",
    description: "Description",
    category: "Custom",
    file: "path/to/custom-tool.html"
  }
];
```

## Performance

- **Size** — ~800 KB total
- **Load Time** — <2 seconds
- **Browser Support** — Chrome, Firefox, Safari, Edge (modern versions)
- **Offline** — Works completely offline after initial load

## Support

See `SETUP.md` for:
- Installation instructions
- Troubleshooting guide
- Deployment options
- Performance optimization

## License

MIT License © 2026 Justice
