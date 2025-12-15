# Zero-Shot Engineering — Specifica Pubblica (v1.0.8)

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

**Zero-Shot Engineering (ZSE)** è un framework di controllo per Large Language Models (LLM) in scenari zero-shot.  
L’obiettivo non è “fare domande migliori”, ma **modellare la distribuzione condizionata** in modo da rendere la generazione più stabile, prevedibile e riutilizzabile.

---

## Stato della Specifica

- **Stato:** Stable  
- **Versione corrente:** v1.0.8  
- **Politica di modifica:**  
  - v1.0.x → chiarimenti, errata, esempi (nessun cambiamento semantico)  
  - v1.x   → estensioni retrocompatibili  
  - v2.0   → cambiamenti non retrocompatibili

---

ZSE si fonda su tre vettori di controllo:

1. **Role Conditioning** – definisce la regione semantica di partenza  
2. **Constraints Injection** – applica vincoli positivi e negativi per ridurre il branching factor  
3. **Output Formatting** – impone vincoli strutturali che rendono l’output altamente vincolato e operativamente prevedibile

Questa repository contiene la **specifica pubblica** di ZSE e alcuni esempi minimi di utilizzo.

---

## 📚 Documentazione

- **Spec in inglese (canonica):** [`docs/en/ZSE-Spec-v1.0.md`](docs/en/ZSE-Spec-v1.0.md)  
- **Spec in italiano (in sviluppo):** [`docs/it/ZSE-Spec-v1.0.it.md`](docs/it/ZSE-Spec-v1.0.it.md)

Esempi:

- [`examples/example_prompt_zse.en.md`](examples/example_prompt_zse.en.md)  
- [`examples/minimal_template.json`](examples/minimal_template.json)

---

## 🎯 Obiettivo

Questa specifica pubblica ha tre scopi principali:

1. **Definire ZSE come disciplina ingegneristica** per il controllo degli LLM.  
2. **Fornire una struttura minima standard** per la costruzione di prompt compatibili con ZSE (ruolo, compito, vincoli, formato di output).  
3. **Offrire una base citabile** per tool, agenti e sistemi multi-modello che adottano ZSE.

La versione completa del whitepaper tecnico (con formalismi matematici, analisi log-probabilistica ed esempi avanzati) è distribuita separatamente come contenuto premium.

---

## 🌍 Lingue

- La documentazione **principale** è in **inglese** (`README.md`, `docs/en/...`).  
- Questa pagina (`README.it.md`) e `docs/it/...` forniscono una versione localizzata per lettori italofoni.

---

## 📜 Licenza

Questa specifica è rilasciata sotto licenza **Creative Commons CC BY-NC-SA 4.0**.

Per i dettagli, vedi il file [`LICENSE`](LICENSE).

---

## 👤 Autore

**Alberto Furnari**  
Senior System Engineer & AI Technical Lead  

- LinkedIn: https://www.linkedin.com/in/alberto-furnari-97695028  
- Newsletter: https://albertofurnari.substack.com  

