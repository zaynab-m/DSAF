# Digital Sovereignty Audit Framework (DSAF) — Operational Reversibility

An open-source audit framework to assess whether an organization can exit its current cloud provider arrangement without catastrophic loss of continuity, data, or institutional knowledge.

The guiding question, from the DICTU Toetsingsinstrument (2026, Criterion 3.4):

> "Can a third party take over the service upon provider failure or contract termination, based on available documentation and design?"

The EuroStack framework (2025, Criterion 2.3) adds:

> "A contractually binding exit plan is mandatory."

**Live site:** https://zaynab-m.github.io/DSAF/

## What's in this repository

- [`index.html`](index.html), [`style.css`](style.css) — the static landing page
- [`assets/DSAF-Operational-Reversibility-v1.1.xlsx`](assets/DSAF-Operational-Reversibility-v1.1.xlsx) — the assessment tool (Excel workbook)
- [`assets/DSAF-diagram.png`](assets/DSAF-diagram.png) — workflow diagram

## The assessment tool

The Excel workbook contains:

| Sheet | Contents |
|---|---|
| `Instructions` | How to use the form, step-by-step workflow, scoring guidance |
| `Definitions` | Glossary of terms (RTO, IaC, tabletop exercise, etc.) |
| `C1` | Exit Plan & Contractual Framework |
| `C2` | Data Portability & Technical Exportability |
| `C3` | Knowledge Transfer & Operational Documentation |
| `C4` | Continuity of Operations During Migration |
| `C5` | Testing Programme & Periodic Evaluation |
| `Summary` | Auto-calculated overall scores and decision rules |

Each control area is assessed on two independent dimensions:

- **Design Maturity (M1–M5)** — is the control designed to achieve its objective?
- **Operating Effectiveness (E1–E4)** — did the designed control actually operate as intended?

The five maturity levels correspond directly to the five DICTU sovereignty levels for Criterion 3.4.

## Running the site locally

This is a fully static site with no build step.

```bash
git clone https://github.com/zaynab-m/DSAF.git
cd DSAF
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploying to GitHub Pages

1. Push this repository to GitHub.
2. In **Settings → Pages**, set the source branch to `main` and the folder to `/ (root)`.
3. The site will be published at `https://<your-username>.github.io/DSAF/`.

## Contributing

Issues and pull requests are welcome — for corrections to the audit criteria, additional control areas, translations, or improvements to the site itself.

## Citing this work

DSAF was developed as part of a master's thesis at Leiden University.

> Musawi, Z. (2026). *Auditing Digital Sovereignty: Design and Evaluation of an Operational Reversibility Framework for IT Auditors* [Unpublished master's thesis]. Leiden University.

```bibtex
@mastersthesis{musawi2026dsaf,
  author = {Musawi, Zaynab},
  title  = {Auditing Digital Sovereignty: Design and
            Evaluation of an Operational Reversibility
            Framework for IT Auditors},
  school = {Leiden University},
  year   = {2026},
  note   = {Unpublished master's thesis}
}
```

## Contact & collaboration

DSAF was developed by Zaynab Musawi, MSc student in ICT in Business and the Public Sector at Leiden University. Feedback, pilot collaborations, and contributions to the framework are welcome.

- LinkedIn: [linkedin.com/in/zaynab-musawi](https://www.linkedin.com/in/zaynab-musawi)
- Issues: [github.com/zaynab-m/DSAF/issues](https://github.com/zaynab-m/DSAF/issues)

## License

Released under the [MIT License](LICENSE). Free to use, adapt, and redistribute, including for commercial audits, provided the copyright notice is retained.

## Framework sources

The sovereignty dimensions, control objectives, and structure of this framework are derived from DICTU, relevant ISO standards, the EuroStack Buy European Framework, and broader sovereignty frameworks, consolidated and operationalized into auditable control language for IT auditing in the context of operational reversibility.
