# Interactive Assessment Tools Bundle — Setup Instructions

## Initial Setup

### 1. Copy Tool Files

From `D:\LLMComplianceSkill\tools\interactive\`, copy all `.html` files:

```bash
# Copy all interactive tool HTML files
cp D:\LLMComplianceSkill\tools\interactive\*.html ./tools/

# Copy shared JavaScript library
cp D:\LLMComplianceSkill\tools\interactive\shared.js ./shared.js
```

### 2. Directory Structure After Copy

```
compliance-assessment-tools/
├── tools/
│   ├── ai-literacy-training.html
│   ├── automated-decision-logic.html
│   ├── bias-testing.html
│   ├── conformity-assessment.html
│   ├── consent-design.html
│   ├── consent-records-audit.html
│   ├── content-labeling.html
│   ├── content-moderation.html
│   ├── disclosure-toolkit.html
│   ├── dsr-rights-implementation.html
│   ├── governance-framework.html
│   ├── human-oversight.html
│   ├── impact-risk-scoring.html
│   ├── incident-management.html
│   ├── llm-selector.html
│   ├── pia-assessment.html
│   ├── risk-classification.html
│   ├── security-assessment.html
│   ├── supply-chain-risk.html
│   ├── training-data-disclosure.html
│   └── transparency-documentation.html
├── shared.js                          # Shared library for all tools
├── index.html                         # Launcher/discovery page
├── package.json
├── README.md
├── SETUP.md                           # This file
└── LICENSE
```

## Running the Tools

### Option 1: Using npm serve

```bash
npm install
npm run serve
```

Then open: http://localhost:3000

### Option 2: Using http-server

```bash
npm run dev
```

Then open: http://localhost:8000

### Option 3: Direct File Access

Open `index.html` directly in your browser:
```bash
# On Windows
start index.html

# On Mac
open index.html

# On Linux
xdg-open index.html
```

## Tool Categories

### Assessment & Scoring (4 tools)
- Impact & Risk Scoring
- Risk Classification
- Privacy Impact Assessment
- Conformity Assessment

### Privacy & Consent (4 tools)
- Consent Design
- Consent Records Audit
- Data Subject Rights Implementation
- Privacy Impact Assessment

### Disclosure & Transparency (4 tools)
- Disclosure Toolkit
- Content Labeling
- Training Data Disclosure
- Transparency Documentation

### Risk & Security (3 tools)
- Incident Management
- Supply Chain Risk
- Security Assessment

### Systems & Operations (3 tools)
- Automated Decision Logic
- Content Moderation
- Human Oversight Design

### Support (2 tools)
- AI Literacy Training
- LLM Model Selector
- Governance Framework

## Customization

### Modifying index.html

To change the tool list, edit the `tools` array in the `<script>` section:

```javascript
const tools = [
  {
    name: "Tool Name",
    description: "Tool description",
    category: "Category",
    file: "path/to/tool.html"
  },
  // ... more tools
];
```

### Updating shared.js

If you modify shared.js, all tools that depend on it will automatically use the new version.

## Deployment

### Static Hosting

These tools can be deployed to any static web host:

```bash
# Build/prepare (optional)
npm install

# Deploy the entire directory to your host
# All files in this directory are static HTML/JS/CSS
```

Supports:
- GitHub Pages
- Netlify
- Vercel
- AWS S3
- Any static file server

### Docker (Optional)

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
```

## Troubleshooting

### Tools not loading

1. Verify all `.html` files are in `tools/` directory
2. Check that filenames in `index.html` match actual file names
3. Ensure `shared.js` is in root directory
4. Check browser console for errors (F12)

### "shared.js not found"

Run setup again to copy the file:
```bash
cp D:\LLMComplianceSkill\tools\interactive\shared.js ./shared.js
```

### Port already in use

Change the port when running:
```bash
npx serve . -p 3001
npx http-server . -p 8001
```

## Performance Notes

- All tools are client-side (no server required)
- Works offline once loaded
- Lightweight (~800KB total)
- Responsive design works on mobile and desktop

## Next Steps

1. Open `index.html` in your browser
2. Try each tool in your compliance category
3. Export results for documentation
4. Integrate findings into compliance reports
