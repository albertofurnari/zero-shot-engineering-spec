# Zero-Shot Engineering — Public Specification (v1.0.8)

![ZSE Spec Version](https://img.shields.io/badge/ZSE_Spec-v1.0-blue.svg)
![Status](https://img.shields.io/badge/status-stable-brightgreen.svg)
![Latest Release](https://img.shields.io/github/v/release/albertofurnari/zero-shot-engineering-spec)
![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)
![Discipline](https://img.shields.io/badge/discipline-LLM%20Control%20Patterns-yellow.svg)
![Docs: EN](https://img.shields.io/badge/docs-English-blue)
![Docs: IT](https://img.shields.io/badge/docs-Italian-orange)
![Framework](https://img.shields.io/badge/type-LLM%20Control%20Framework-purple.svg)
[![DOI](https://zenodo.org/badge/1114291456.svg)](https://doi.org/10.5281/zenodo.17909367)
![GitHub Sponsors](https://img.shields.io/badge/sponsor-on%20github-ff69b4.svg)
![Dark Minimal](https://img.shields.io/badge/style-minimal-black.svg)

**Zero-Shot Engineering (ZSE)** is a constraint-based framework for controlling Large Language Models (LLMs) in zero-shot settings.  
The goal is not to “ask better questions”, but to **shape the conditional distribution** so that generation becomes more stable, predictable, and reusable.

---

## Specification Status

- **Status:** Stable  
- **Current version:** v1.0.8  
- **Change policy:**  
  - v1.0.x → clarifications, errata, examples (no semantic changes)  
  - v1.x   → backward-compatible extensions  
  - v2.0   → breaking changes

---

ZSE is built on three core control vectors:

1. **Role Conditioning** – defines the initial semantic subspace  
2. **Constraints Injection** – applies positive and negative constraints to reduce the branching factor  
3. **Output Formatting** – enforces structural “cages” that make generation highly constrained and operationally predictable

This repository contains the **public specification** of ZSE and a minimal set of examples.

---

## Normative Scope

This repository defines the **normative specification** of Zero-Shot Engineering.

The following concepts are **normative** and must be interpreted exactly as defined
in the specification:

- Zero-Shot Engineering (ZSE)
- Role Conditioning
- Constraints Injection
- Output Formatting
- Branching Factor (operational proxy)

Any use of the term “ZSE” that contradicts these definitions
does not conform to this specification.

---

## 📚 Documentation

- **English spec**: [`docs/en/ZSE-Spec-v1.0.md`](docs/en/ZSE-Spec-v1.0.md)  
- **Italian spec (work in progress)**: [`docs/it/ZSE-Spec-v1.0.it.md`](docs/it/ZSE-Spec-v1.0.it.md)

Examples:

- [`examples/example_prompt_zse.en.md`](examples/example_prompt_zse.en.md)  
- [`examples/minimal_template.json`](examples/minimal_template.json)

---

## 🎯 Purpose

The ZSE public specification aims to:

1. **Define Zero-Shot Engineering as an engineering discipline** for LLM control patterns.  
2. **Provide a minimal standard structure** for ZSE-compatible prompts (role, task, constraints, output format).  
3. **Offer a citable reference** for tools, agents, and multi-model systems that adopt ZSE.

The full technical whitepaper (with mathematical formalism, log-probability analysis, and advanced case studies) is distributed separately as premium content.

---

## 🌍 Languages

- **Primary language:** English (`README.md`, `docs/en/...`)  
- **Italian version:** [`README.it.md`](README.it.md) and `docs/it/...`

Both versions describe the same framework; the English one is considered canonical for citation.

---

## 🛠️ Contributions & Governance

This repository hosts a **technical specification**, not a discussion draft.

Accepted contributions:
- Errata and clarifications
- Examples and tooling
- Editorial improvements

Rejected contributions:
- Semantic reinterpretations
- Renaming of core concepts
- Changes to axioms without a major version bump

Final decisions on wording, scope, and versioning
rest with the maintainer to preserve semantic coherence.

---

## 📜 License

This public specification is released under the **Creative Commons CC BY-NC-SA 4.0** license.

- **BY** – You must attribute the work to **Alberto Furnari**  
- **NC** – No direct commercial use  
- **SA** – Derivative works must keep the same license

See [`LICENSE`](LICENSE) for details.


---

## How to cite

Furnari, A. (2025). *Zero-Shot Engineering — Public Specification (v1.0)*. Zenodo.
https://doi.org/10.5281/zenodo.17909367

---

## 👤 Author

**Alberto Furnari**  
Senior System Engineer & AI Technical Lead  

- LinkedIn: https://www.linkedin.com/in/alberto-furnari-97695028  
- Newsletter: https://albertofurnari.substack.com  

Issues and suggestions for improvement are welcome.

