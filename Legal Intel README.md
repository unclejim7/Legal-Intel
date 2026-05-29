# ⚖️ Legal Intel — AI × Workers’ Compensation & Personal Injury Law

> *“All the intelligence that’s fit to argue.”*

A daily AI-powered briefing publication for workers’ compensation and personal injury attorneys, delivered in the aesthetic of a classic legal broadsheet. Built on Claude + web search. Run it once a day. Stay ahead of the practice.

-----

## What It Is

**Legal Intel** is a Claude Project + React/HTML application that produces a fully formatted, newspaper-style daily intelligence brief covering:

- AI tool launches and product news for WC/PI legal practice
- Case law and regulatory developments from WCAB, state boards, and appellate courts
- Medical and expert witness AI developments affecting causation and damages arguments
- Agentic AI workflow developments for law firms
- ABA and state bar ethics guidance on AI use
- Curated daily resources (CLEs, papers, tools)
- Strategic takes for practitioners and founders building in this space

-----

## Quick Start

### Option 1 — Claude Project (Recommended, No Code)

1. Open [claude.ai](https://claude.ai)
1. Create a new **Project**
1. Name it: `Legal Intel`
1. Paste the contents of [`CLAUDE_PROJECT_INSTRUCTIONS.md`](./CLAUDE_PROJECT_INSTRUCTIONS.md) into the Project Instructions field
1. Each morning, open the project and type:

```
run legal
```

Claude runs a full web-searched brief and outputs 3 files: `index.html`, `YYYY-MM-DD.html`, and `archive.html`.

-----

### Option 2 — Standalone HTML App

The `src/LegalIntel.jsx` file is a standalone React component that renders the brief in a full broadsheet newspaper layout with live Claude API calls. The `legal-intel.html` file is a zero-dependency single-file version.

**Run locally:**

```bash
git clone https://github.com/unclejim7/legal-intel
cd legal-intel
npm install
npm run dev
```

-----

## GitHub Pages Deployment

After each `run legal` execution, upload the 3 generated files to your repo:

|File             |URL                                                      |
|-----------------|---------------------------------------------------------|
|`index.html`     |`https://unclejim7.github.io/legal-intel`                |
|`YYYY-MM-DD.html`|`https://unclejim7.github.io/legal-intel/YYYY-MM-DD.html`|
|`archive.html`   |`https://unclejim7.github.io/legal-intel/archive.html`   |

Enable GitHub Pages in repo Settings → Pages → Deploy from branch: `main`, folder: `/ (root)`.

-----

## Project Structure

```
legal-intel/
├── README.md
├── CLAUDE_PROJECT_INSTRUCTIONS.md
├── legal-intel.html                   # Standalone single-file app
├── src/
│   └── LegalIntel.jsx                 # React component version
├── package.json
├── vite.config.js
└── .github/
    └── workflows/
        └── legal-intel-daily.yml
```

-----

## Trigger Word

In any Claude Project using these instructions, type:

```
run legal
```

Claude executes the full daily brief — no preamble, no filler, straight to the edition.

-----

## Coverage Areas

|Section                      |What It Covers                                                  |
|-----------------------------|----------------------------------------------------------------|
|Above the Fold               |Lead story — biggest AI/legal development of the day            |
|Today’s Headlines            |3–5 news items with practitioner angle                          |
|Tool Spotlight               |Deep dive on one AI tool for WC/PI practice                     |
|The Agentic Corner           |Agentic AI workflow developments for legal                      |
|Case Law & Regulatory Radar  |WCAB decisions, appellate opinions, board guidance, ABA ethics  |
|Medical & Expert Intelligence|IME AI, medical imaging, surveillance tech, expert methodologies|
|Resource of the Day          |Article, CLE, paper, repo, or tool worth your time              |
|Editor’s Dispatch            |3 sharp analytical observations                                 |

-----

## Design

Legal Intel is styled after classic legal and financial broadsheets with:

- Masthead with edition number and date
- Multi-column broadsheet layout
- Serif body typography (Playfair Display + EB Garamond)
- Above-the-fold lead story
- Deep navy / cream / gold ink palette — legal gravitas
- Section dividers and column rules

-----

## Stack

|Layer   |Tech                                        |
|--------|--------------------------------------------|
|AI      |Claude Sonnet 4 via Anthropic API           |
|Search  |web_search_20250305 tool                    |
|Frontend|React + vanilla CSS / standalone HTML       |
|Fonts   |Playfair Display, EB Garamond (Google Fonts)|
|Deploy  |GitHub Pages                                |

-----

## Disclaimer

Legal Intel is not legal advice. All content is AI-generated and should be independently verified. Not affiliated with any bar association or legal publisher.

-----

## License

MIT — fork it, build on it, publish your own edition.

-----

*Legal Intel. Est. 2025. All the intelligence that’s fit to argue.*