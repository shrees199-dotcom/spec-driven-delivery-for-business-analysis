# Project Structure

This repository is organized to keep the BA governance workflow repeatable and auditable.

## Root layout

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

## Purpose of each directory

### `docs/`

Contains BA process guidance and workflow references.

### `skills/`

Hosts the actual prompt files for the two skills used in the governance model.

### `templates/`

Stores reusable file templates that map directly to the workflow artifacts.

## Template files

### `templates/narrative.md`
Plain-language narrative record as captured from stakeholder discussion.

### `templates/contract.json`
Structured, build-ready contract with confidence levels and open-item tracking.

### `templates/golden_dataset.yaml`
Answer key with example situations and expected results.

### `templates/eval_report.yaml`
Grading record with pass/fail results and routing of fixes.

## Recommended usage

1. Use `skills/narrative-extraction-node.md` for discovery analysis
2. Use `skills/spec-driven-node-v3.md` for contract and grading governance
3. Copy relevant templates when creating a new capability spec
4. Keep all outputs in the same repo for evidence continuity
