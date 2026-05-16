# Testing Beyond Automation - Version 1.0 Initial Proposal Draft

**Title:** Testing Beyond Automation: Evidence, Doubt, and Operational Risk in the Age of Generative AI  
**Subtitle:** Toward an Evidence-Centric, Observability-Driven Assurance Model for Complex Identity and Biometric Systems  
**Author:** Guillaume Harbonnier  
**Status:** Initial proposal draft. Not peer reviewed.

<p align="center">
  <a href="./Whitepaper_PDF_v1_0_initial_draft.pdf">
    <img src="https://img.shields.io/badge/Open-White%20Paper-0B5FFF?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="View PDF">
  </a>
</p>

## Purpose

This is the first public-style proposal release of the whitepaper. It is intentionally framed as a draft for critique, discussion, pilot implementation, and future refinement — not as a peer-reviewed publication.

## Core thesis

Generative AI can industrialize testing variability, but it should not replace test thinking.

The strategic value of testing lies in:

- doubt,
- priors,
- confronting unknowns,
- architecture challenge,
- epistemic reasoning,
- requirements treated as hypotheses,
- assumptions treated as governed risk objects,
- human-defined truth,
- telemetry as oracle,
- AI-assisted verification of governed controls,
- generated generators,
- evidence-based operational assurance.

## Key clarifications in v1.0

1. The paper is labeled **Version 1.0 - Initial Proposal Draft - Not Peer Reviewed**.
2. It removes internal changelog language such as "final reference and editorial edition" from the abstract.
3. It clarifies that many requirements are operational hypotheses.
4. It distinguishes assumptions from hypotheses using a falsifiability rule.
5. It explains that assumptions require a risk/exposure score: `R0 = P(Assumption False) × Impact × DependencyMultiplier`.
6. It clarifies where a prior value such as `P(Claim Valid)=0.70` comes from.
7. It connects prior confidence to historical data, expert elicitation, architecture review, incident history, and STRAT-Q-style risk models.
8. It keeps the Bayesian example but makes the prior provenance explicit.

## Repository structure

```text
.
├── README.md
|── LICENSE-APACHE-2.0.md
|── LICENSE-CC-BY-SA-4.0.md
├── paper/
│   ├── main.tex
│   └── main.pdf
├── appendix/
│   ├── generator_spec.yaml
│   ├── trace_validation_rule.yaml
│   └── evidence_record_example.json
└── diagrams/
    └── workflow.mmd
```

## Build

From the `paper/` directory:

```bash
pdflatex main.tex
pdflatex main.tex
```
