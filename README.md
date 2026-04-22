# Prompt//Shield — AI Security Education Platform

> A complete, self-contained educational website covering AI security, prompt injection attacks, adversarial machine learning, governance, and defence-in-depth strategies — built for cybersecurity practitioners, AI engineers, and students.

-----

## 📁 Project Structure

```
prompt-shield/
├── ai-security-education.html   ← Main course page (start here)
├── curriculum.html              ← 3-Day structured curriculum overview
├── textbook.html                ← Full textbook with 20+ chapters + 20 videos
└── README.md                    ← This file
```

All four files are standalone HTML — no build step, no dependencies, no server required. Open any file directly in a modern browser.

-----

## 🗂️ File Descriptions

### `ai-security-education.html` — Main Course Page

The primary entry point for the platform. Contains:

- **Hero landing section** introducing the course mission
- **Module 00 — Learning Objectives**: 6 competency-based outcomes aligned to Bloom’s Taxonomy
- **Module 01 — Attack Taxonomy**: 7 expandable attack cards covering direct injection, indirect/environmental injection, encoding obfuscation, persona jailbreaking, steganographic output attacks, context window manipulation, and prompt leakage — each with real examples and mitigations
- **Module 02 — Defense-in-Depth Framework**: 5-layer model (Input → Context → Model → Output → Architecture) based on OWASP LLM Top 10 and NIST AI RMF principles
- **Module 03 — Pedagogical Framework**: Learning theory foundations (Kolb, Bloom, Red/Blue teaming, Threshold Concepts)
- **Module 04 — Progression Levels**: 5 CTF-style levels from novice to expert
- **Module 05 — Ethical Responsibilities**: Responsible disclosure, authorisation requirements, ACM Code of Ethics
- **Module 06 — External Resources**: 11 curated video and reference cards linking to YouTube talks, OWASP documentation, Gandalf CTF, and Simon Willison’s blog

**Navigation links to:** `curriculum.html`, `textbook.html`

-----

### `curriculum.html` — 3-Day Curriculum Overview

A structured course outline presenting all sessions, topics, and lab exercises across the 3-day intensive programme. Contains:

- **Hero stats bar**: 3 days · 6 sessions · 12+ hands-on labs · 4 frameworks
- **Sticky sidebar navigation** with jump-links to every session
- **Day 1 — Foundations & Methodology**: Threat modelling, AI-DICE framework, DFDs, STRIDE-AI, attack trees with Mermaid
- **Day 2 — Implementation & Defence**: Attack simulation, OWASP Top 10 for LLMs, MITRE ATLAS, OWASP AI Exchange, security-by-design, risk assessment
- **Day 3 — Advanced Concepts**: EU AI Act & GDPR, ethics & explainability, privacy-by-design, MLOps security, AI DevSecOps, final red/blue team wargame
- **Topic cards** distinguish regular topics from hands-on labs (green-highlighted) and the capstone wargame (red-highlighted)
- **Framework chips** throughout showing OWASP, MITRE ATLAS, EU AI Act, STRIDE-AI, and other referenced standards
- **CTA banner** linking to the textbook

**Navigation links to:** `textbook.html`, `ai-security-education.html`

-----

### `textbook.html` — Full Textbook Edition

The comprehensive educational reference for all 3 days of content. The most content-rich file in the project. Contains:

**20+ chapters of textbook content:**

|Chapter|Topic                                                                     |
|-------|--------------------------------------------------------------------------|
|1.1    |What is AI Threat Modelling? (NIST AI RMF, 4-question framework)          |
|1.2    |Traditional vs. AI Threat Modelling (comparative definition table)        |
|1.3    |The AI-DICE Framework (Data / Inference / Control / Exposure)             |
|1.4    |Data Flow Diagramming for AI (Mermaid DFD example)                        |
|1.5    |STRIDE-AI Taxonomy (full 6-category table with AI manifestations)         |
|1.6    |Core AI Attack Classes (injection, poisoning, theft, jailbreaking)        |
|1.7    |Attack Trees & Mermaid (with example attack tree)                         |
|2.1    |AI Attack Scenario Analysis (real-world case studies)                     |
|2.2    |OWASP Top 10 for LLM Applications 2025                                    |
|2.3    |MITRE ATLAS (16 tactics, 84 techniques, 6 key technique profiles)         |
|2.4    |OWASP AI Exchange & MIT AI Risk Library                                   |
|2.5    |Security by Design (model lifecycle, data pipeline, API hardening)        |
|2.6    |AI Risk Assessment (OWASP risk rating, risk matrices)                     |
|3.1    |EU AI Act — 4-tier risk classification (with Article citations)           |
|3.2    |AI Ethics, Explainability & Bias Mitigation (SHAP, LIME, fairness metrics)|
|3.3    |Privacy-by-Design (Differential Privacy, Federated Learning, DP-SGD)      |
|3.4    |Securing MLOps & AI DevSecOps Pipelines (AI-BOM, MLSecOps)                |
|3.5    |Security Incident Handling for AI Systems                                 |
|3.6    |Red/Blue Team Wargame Methodology                                         |

**20 curated video resources** embedded at the end of each day, mapped to specific chapters:

- Day 1: 6 videos on threat modelling, STRIDE, and AI attack classes
- Day 2: 8 videos on OWASP LLM Top 10, MITRE ATLAS, and security by design
- Day 3: 9 videos on the EU AI Act, AI bias/XAI, federated learning/DP, and MLOps security

**Navigation links to:** `curriculum.html`, `ai-security-education.html`

-----

## 🔗 Site Navigation Map

```
ai-security-education.html  (Main Course)
    │
    ├──► curriculum.html  (3-Day Curriculum)
    │        │
    │        └──► textbook.html  (Full Textbook)
    │                 │
    │                 └──► [back links to all pages]
    │
    └──► textbook.html  (direct link from nav + CTA banner)
```

All pages contain full cross-linking in both the sticky navigation bar and inline CTA sections, so users can move freely between all three views.

-----

## 🎨 Design System

All three pages share a consistent visual identity:

|Token      |Value          |Usage                     |
|-----------|---------------|--------------------------|
|`--bg`     |`#0a0c10`      |Page background           |
|`--surface`|`#0f1218`      |Card backgrounds          |
|`--accent` |`#00e5ff`      |Day 1 / primary cyan      |
|`--accent2`|`#ff4d6d`      |Day 2 / warnings / attacks|
|`--accent3`|`#a3f7bf`      |Day 3 / defences / green  |
|`--warn`   |`#ffbe0b`      |Labs / video resources    |
|`--purple` |`#c77dff`      |Governance / ethics       |
|`--mono`   |Share Tech Mono|Code, labels, metadata    |
|`--display`|Syne           |Headings, titles          |
|`--body`   |DM Sans        |Body copy                 |

**Visual effects:** CRT scanline overlay (CSS `repeating-linear-gradient`), grid background in hero sections, sticky glassmorphism nav, animated pulse borders.

**Fonts loaded from:** Google Fonts CDN (Share Tech Mono, Syne, DM Sans). An internet connection is required to load fonts; pages are fully functional without them (system monospace/sans-serif fallback applies).

-----

## 📚 Frameworks & Standards Referenced

|Framework                                 |Coverage                                            |
|------------------------------------------|----------------------------------------------------|
|**STRIDE-AI**                             |Chapter 1.5, Day 1 afternoon session                |
|**OWASP Top 10 for LLM Applications 2025**|Chapter 2.2, Module 01 attack cards                 |
|**MITRE ATLAS v5.1.0**                    |Chapter 2.3 (16 tactics, 84 techniques)             |
|**OWASP AI Exchange**                     |Chapter 2.4                                         |
|**MIT AI Risk Repository**                |Chapter 2.4                                         |
|**NIST AI RMF**                           |Chapter 1.1, Defense Framework Module 02            |
|**EU AI Act (Reg. 2024/1689)**            |Chapter 3.1 (all 4 risk tiers, Articles 5, 9–15, 73)|
|**GDPR Articles 5, 22, 25, 35**           |Chapter 3.1, 3.3                                    |

-----

## ⚖️ Ethical Use Statement

This platform is designed exclusively for **defensive security education**. All attack examples are drawn from published academic research and documented real-world incidents for the purpose of teaching practitioners how to recognise, understand, and prevent them.

- All hands-on lab exercises use **synthetic secrets in sandboxed environments**
- Users are expected to apply these techniques **only against systems they own or have explicit written authorisation to test**
- The platform operates under the **ACM Code of Ethics** and a **responsible disclosure framework**
- Knowledge of attack techniques is presented to enable better defence — not to facilitate harm

See **Module 05 — Ethical Responsibilities** in `ai-security-education.html` for the full ethical framework.

-----

## 🛠️ Technical Requirements

|Requirement      |Details                                                             |
|-----------------|--------------------------------------------------------------------|
|**Browser**      |Any modern browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)  |
|**Server**       |None required — open HTML files directly                            |
|**Dependencies** |Google Fonts CDN (graceful fallback if unavailable)                 |
|**JavaScript**   |Minimal vanilla JS (accordion toggle only) — no frameworks          |
|**CSS**          |Pure CSS, no preprocessor — uses CSS custom properties              |
|**Accessibility**|Semantic HTML structure; colour contrast meets WCAG AA for body text|

-----

## 📖 Recommended Reading Order

**For new students:**

1. Start at `ai-security-education.html` → read the Attack Taxonomy (expand all cards)
1. Move to `curriculum.html` → review the 3-day schedule and lab overview
1. Open `textbook.html` → read Day 1 chapters, then watch the Day 1 videos
1. Return daily for Days 2 and 3 content

**For experienced practitioners:**

1. Jump directly to `textbook.html` using the sidebar navigation
1. Use the STRIDE-AI table (Ch 1.5) and MITRE ATLAS section (Ch 2.3) as quick references
1. Cross-reference the EU AI Act tier table (Ch 3.1) for compliance work

**For instructors:**

1. Use `curriculum.html` as the student-facing course syllabus
1. Use `textbook.html` chapters as pre-reading assignments ahead of each session
1. The lab exercises (green-highlighted in the curriculum) map directly to the concept boxes and case studies in the textbook

-----

## 🔖 Citation & Attribution

Academic sources cited throughout the textbook include:

- Mauri, L. & Damiani, E. (2022). *STRIDE-AI: An Approach to Identifying Vulnerabilities of Machine Learning Assets*. PMC/NIH; IEEE RTSI 2025.
- OWASP Foundation (2024). *Top 10 for LLM Applications 2025*. genai.owasp.org
- MITRE Corporation (2025). *ATLAS v5.1.0 — Adversarial Threat Landscape for AI Systems*. atlas.mitre.org
- European Union (2024). *Artificial Intelligence Act, Regulation (EU) 2024/1689*. Official Journal, 12 July 2024.
- NIST (2023). *AI Risk Management Framework (AI RMF 1.0)*. nist.gov/airmf
- JFrog (2025). *Software Supply Chain State of the Union 2025*.
- OpenSSF (2025). *MLSecOps Whitepaper*.

-----

*Prompt//Shield — Built for defenders.*