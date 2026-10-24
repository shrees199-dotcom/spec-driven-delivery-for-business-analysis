# Spec-Driven Delivery for Business Analysis

A reusable BA operating model for turning raw stakeholder discovery into validated, buildable delivery work.

This project packages two complementary skills into a single workflow:

- Narrative Extraction Analyst
- Spec-Driven Delivery Governor

Together, they create a disciplined process that moves from unstructured discovery material to a contract that is precise enough for engineering and testable enough for QA.

## Why this project exists

Business discovery often stays in conversation form long enough that teams begin filling in gaps with assumptions. That creates avoidable rework, bad builds, and weak validation.

This project encodes a higher standard:

- only real stakeholder input becomes a requirement
- ambiguity is tracked honestly instead of guessed away
- contracts are written in a precise, buildable form
- answer keys are created before implementation
- real build output is required before grading
- failures are routed to either the contract or the build, not both

## Core workflow

1. Ingest raw discovery material session by session
2. Separate topics into distinct capabilities
3. Label each as Confirmed, Exploratory, or Rejected
4. Hand only confirmed narratives to the governor
5. Draft a strict Contract
6. Batch unresolved items into a Stakeholder Question Packet
7. Create a Golden Dataset before implementation
8. Halt until a real build reports actual outputs
9. Grade the real outputs against the Answer Key
10. Route each failure accurately

## Included assets

- `skills/narrative-extraction-node.md` — the discovery extraction skill
- `skills/spec-driven-node-v3.md` — the contract, answer-key, and grading skill
- `docs/ba-workflow.md` — operational workflow for BAs and delivery teams
- `docs/project-structure.md` — repository structure and usage
- `templates/narrative.md` — plain-language narrative template
- `templates/contract.json` — contract schema template
- `templates/golden_dataset.yaml` — answer key template
- `templates/eval_report.yaml` — grading template

## Folder structure

```text
.
├── README.md
├── docs/
│   ├── ba-workflow.md
│   └── project-structure.md
├── skills/
│   ├── narrative-extraction-node.md
│   └── spec-driven-node-v3.md
├── templates/
│   ├── contract.json
│   ├── eval_report.yaml
│   ├── golden_dataset.yaml
│   └── narrative.md
└── .gitignore
```

## Intended use

This is designed for teams that want a durable BA-to-engineering-to-QA pipeline with visible evidence instead of assumptions.

Use it for:

- feature discovery and requirement clarification
- contract drafting for AI and software features
- BA sign-off and stakeholder question batching
- test planning before build work starts
- evidence-based grading of real output

## Important principle

The process refuses invented stakeholder answers. A requirement is only valid when it is real, stated, or clearly flagged as provisional with the BA's reasoning attached.

## License

MIT

## Project status

This repo contains the specification package and project scaffolding for the BA-driven spec governance model.
