# Setup

## 1. Repository

Create or use the public profile repository:

`aviicroft/aviicroft`

GitHub profile repositories must match the account username.

## 2. Copy the files

Keep this structure:

```text
aviicroft/
├── README.md
├── assets/
│   ├── hero.svg
│   ├── cyber-network.svg
│   ├── blockchain-trace.svg
│   ├── ai-pipeline.svg
│   ├── cloud-pipeline.svg
│   ├── terminal.svg
│   └── divider.svg
└── .github/
    └── workflows/
        └── contribution-snake.yml
```

## 3. Enable the contribution animation

Push the repository to GitHub, then run:

**Actions → Generate Contribution Snake → Run workflow**

The workflow publishes the generated SVG to the `output` branch.

## 4. GitHub statistics

The README uses dynamic image endpoints for:

- GitHub statistics
- Top languages
- GitHub streak
- Contribution snake

No statistics are hard-coded.

## 5. Customization

The visual system is intentionally centralized in the SVG assets.

Primary palette:

- Background: near-black
- Cyan: `#00e5ff`
- Red: `#ff244f`
- Terminal green: `#59ff9a`

Animation uses SVG/SMIL only. There is no JavaScript, iframe, embedded dashboard, or hover-dependent interaction.

## 6. Important GitHub rendering note

GitHub sanitizes SVG/HTML content. The README therefore references SVG assets as images instead of embedding arbitrary SVG markup directly into the Markdown.

The animated effects are contained inside the SVG files. If a GitHub rendering surface suppresses a particular SMIL animation, the underlying graphic still remains visible as a static fallback.
