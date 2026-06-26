# Payment Trajectories and Causal Delinquency: Predicting Credit Card Default in Taiwan

![Notebook CI](https://github.com/shantanu-777/dai-mission-group-v/actions/workflows/run-notebook.yml/badge.svg)

---

## Team

| Name | Role |
|------|------|
| Tom Skirde | Lead / Causal Inference |
| Shantanu Modhave | Supervised Learning |
| Vritika Kamra | Unsupervised / Generative |

> No student IDs in this file. Submit IDs separately via the course system (Moodle).

---

## Research Question

Do earlier months of payment delinquency causally increase the probability of credit default beyond what the most recent payment behaviour already explains and can we identify distinct **repayment trajectory types** that serve as meaningful risk archetypes?

---

## Methods Overview

| Block | Method(s) |
|-------|-----------|
| Causal Inference | DoWhy — [backdoor / IV / propensity score] |
| Supervised Learning | [e.g., Ridge regression, Random Forest, …] |
| Unsupervised / Generative | [e.g., K-Means, VAE, Hierarchical clustering, …] |

---

## Data Sources

**Dataset** :Source(s):
UCI Machine Learning Repository — Default of Credit Card Clients (Yeh, 2009)
Licence: CC BY 4.0. Original paper: Yeh & Lien, Expert Systems with Applications, 2009.

Unit of observation: One credit card client-month record (30,000 rows, 23 features + 1 target)

**URL:** [Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)

---

## How to Run

### Option A — GitHub Actions (zero local setup)

Push to `main`. The CI workflow executes `notebook.ipynb` automatically.

- Check the **Actions** tab to see whether the run passed or failed.
- Download the `executed-notebook-*` artifact to inspect all cell outputs.
- The badge at the top of this README turns green when the notebook runs clean.

### Option B — Local environment

```bash
# Clone your repo (not this template)
git clone https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>.git
cd <YOUR_REPO_NAME>

python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab notebook.ipynb
```

---

## Presentation Slide Requirements

| Item | Rule |
|------|------|
| Content slides | **Maximum 5** |
| Allowed extras | Title page · Literature/Reference slide · Backup slides |
| Backup slide content | Tables or figures/diagrams **only** |
| Required topics | Motivation & Economic Relevance · Data & Methodology · Results · Limitations & Synthesis |
| File format | **PDF only** — do not submit PPTX |
| Delivery | No live presentation — slides are reviewed during the oral exam |

---

## Oral Exam

- **Format:** 15-minute Q&A per group — questions on your Proposal and Presentation slides
- **Individual accountability:** each member answers questions on their own area (see Work Plan in notebook)
- **Rooms:** Morning sessions → M811 · Afternoon sessions → M827 · Arrive 10 minutes early
- **Grading:** oral performance directly modifies your Mission base score; significant individual
  discrepancies lead to differentiated individual grades

---

## Key Deadlines

| Date | Time | What |
|------|------|------|
| June 18 | 12:00 noon | Rank your session slots in Moodle (group lead) |
| June 30 | 12:00 noon | Submit repository link to Moodle (exactly one member per group) |
| June 30 | 23:59 | Final code deadline — commits after this are not graded |

> **Private repositories:** if your repo is private you MUST invite `pnposch` and
> `kiraschoenhuette` as collaborators before the deadline so the teaching team can clone it.

---

## Submission Checklist

| Item | Status |
|------|--------|
| Repo named `dai-mission-group-V` (replace X with your group letter) | [ ] |
| README updated (title, team, badge URL, research question, data sources) | [ ] |
| Work Plan filled in (`notebook.ipynb` — team member → section mapping) | [ ] |
| All rubric sections complete (§1–§5) | [ ] |
| Notebook submitted in **fully executed state** (all cell outputs visible) | [ ] |
| Notebook re-executes cleanly (CI badge green) | [ ] |
| `presentation.pdf` replaced with actual PDF (PDF only, no PPTX) | [ ] |
| Large data files (≥ 100 MB) not committed — downloaded or Sciebo-linked instead | [ ] |
| Custom `.py` modules included (if any) | [ ] |
| Private repo: `pnposch` + `kiraschoenhuette` added as collaborators | [ ] if private |
| Repository link submitted to Moodle by **June 30, 12:00 noon** | [ ] |

---

## Repository Structure

```
.
├── .github/workflows/run-notebook.yml   # CI: validates and executes notebook on every push
├── data/                                # local data files (see data/README.md)
├── notebook.ipynb                       # main deliverable — proposal + final submission (submit fully executed)
├── presentation.pdf                     # slide deck — PDF only, max 5 content slides
├── README.md                            # this file
└── requirements.txt                     # Python dependencies (required)
```
