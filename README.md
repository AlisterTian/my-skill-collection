# My Skill Collection

**English** | [简体中文](README.zh-CN.md)

The research skills I use with AI coding and research assistants: literature discovery, paper writing and review, scientific figures, statistics, bioinformatics, molecular modeling, and laboratory workflows.

This repository shares **170 workflow skills and one shared support package** from my manually installed collection. It preserves local refinements and upstream attribution. Built-in assistant skills and bundled application plugins are not included.

## Find a skill

Browse the **[complete skill catalog](CATALOG.md)** for a short description, use case, and declared license for every included skill. The same index is available as [catalog.json](catalog.json).

| I want to... | Start with |
|---|---|
| Find papers and check references | `paper-lookup`, `nature-academic-search`, `citation-management`, `nature-ref-verifier` |
| Read a paper or understand its evidence | `nature-paper-card`, `nature-reader`, `literature-review` |
| Plan a study and justify sample size | `experimental-design`, `statistical-power`, `hypothesis-generation` |
| Draft, polish, or revise a manuscript | `nature-writing`, `nature-polishing`, `scientific-writing`, `nature-response` |
| Review a paper before submission | `nature-reviewer`, `peer-review`, `nature-statistics` |
| Create figures, posters, or paper presentations | `nature-figure`, `scientific-visualization`, `scientific-slides`, `nature-paper2ppt`, `latex-posters` |
| Analyze data or build a research model | `statistical-analysis`, `pymc`, `scikit-learn`, `pytorch-lightning`, `polars` |
| Analyze sequencing and single-cell data | `bulk-rnaseq`, `scanpy`, `scvi-tools`, `pydeseq2`, `pathway-enrichment` |
| Work with molecules or drug-discovery models | `rdkit`, `deepchem`, `diffdock`, `molecular-dynamics`, `pkpd-modeling` |
| Connect laboratory platforms or record experiments | `benchling-integration`, `opentrons-integration`, `pylabrobot`, `nature-experiment-log` |
| Work across a complete research-to-paper project | `academic-research-suite` |

## Use the collection

1. Open the relevant `skills/<directory>/SKILL.md` and check its prerequisites and supporting references.
2. Copy the selected skill directory into the skill location supported by your assistant, or point the assistant directly at its `SKILL.md`.
3. Keep the directory's scripts, references, templates, and assets together. For Nature skills, also copy `skills/nature-shared` when the selected skill references it. Some workflows refer to other sibling skills; copy those dependencies as needed.
4. Provide the actual research materials and a concrete request. For example:

```text
Use nature-paper-card to analyze this paper and map its experiments to its claims.
Use nature-writing to draft a Results section from these figures and measurements.
Use statistical-power to estimate the sample size for this proposed comparison.
Use scanpy to analyze this single-cell dataset and explain the QC decisions.
```

Skill names can differ from folder names: `researchwrite` lives in `skills/nature-proposal-writer`. The `nature-shared` directory is a dependency, not a standalone workflow.

The repository introduction is available in English and Simplified Chinese; the full catalog is in English. Individual skill instructions retain their original English or Chinese content so established workflows and examples remain usable.

## What this repository contains

```text
skills/              Installed research skill directories and reusable resources
CATALOG.md           Human-readable skill index and use cases
catalog.json         Machine-readable index
LICENSE.md           Component licensing and upstream attribution
licenses/            Retained source-level license texts
MODIFICATIONS.json   Local refinements and publication cleanup
EXCLUDED.md          Installed items and files not redistributed
```

This is a snapshot of the collection I use, not a promise that every API, package, or agent integration is installed or continuously tested. Hosted tools can need their own account, API key, data permissions, or compute budget. Credentials and private research inputs are not included.

## Credits and licensing

Many skills come from [Scientific Agent Skills by K-Dense](https://github.com/K-Dense-AI/scientific-agent-skills), [Nature Skills](https://github.com/Yuan1z0825/nature-skills), and [Academic Research Skills](https://github.com/Imbad0202/academic-research-skills). This repository curates those materials and retains local adjustments; it does not claim original authorship of the upstream skills.

**Licenses vary by component.** See [LICENSE.md](LICENSE.md) and each skill's own notices before reuse. Restricted or unresolved-license items are listed in [EXCLUDED.md](EXCLUDED.md), rather than republished under a blanket license.
