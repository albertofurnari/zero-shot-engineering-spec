# Zero-Shot Engineering — Specifica Pubblica (v1.1.0)

![ZSE Spec Version](https://img.shields.io/badge/ZSE_Spec-v1.1.0-blue.svg)
![Status](https://img.shields.io/badge/status-stable-brightgreen.svg)
![Latest Release](https://img.shields.io/github/v/release/albertofurnari/zero-shot-engineering-spec)
![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)
![Discipline](https://img.shields.io/badge/discipline-LLM%20Control%20Patterns-yellow.svg)
![Docs: EN](https://img.shields.io/badge/docs-English-blue)
![Docs: IT](https://img.shields.io/badge/docs-Italian-orange)
![Type](https://img.shields.io/badge/type-Technical%20Specification-purple.svg)
[![DOI](https://zenodo.org/badge/1114291456.svg)](https://doi.org/10.5281/zenodo.17909367)
![Style](https://img.shields.io/badge/style-minimal-black.svg)

**Zero-Shot Engineering (ZSE)** è una **specifica tecnica** per il controllo inference-time dei Large Language Models (LLM) in scenari zero-shot.  
L’obiettivo non è “fare domande migliori”, ma **modellare la distribuzione condizionata** per ottenere generazioni più stabili, prevedibili e verificabili.

> ⚠️ **Nota di accesso**  
> La **specifica tecnica completa (PDF)** è distribuita separatamente e **non è pubblicamente disponibile** in questo repository.

---

## Stato della Specifica

- **Stato:** Stable  
- **Versione corrente:** v1.1.0  
- **Distribuzione:** controllata (paywall)  
- **Repository role:** supporto pubblico e indice tecnico

### Politica di versioning (spec-oriented)
- **PATCH (x.y.z)** → correzioni editoriali  
- **MINOR (x.y.0)** → chiarimenti normativi  
- **MAJOR (x.0.0)** → cambiamenti non retrocompatibili

---

## Cosa contiene questo repository

Questo repository **NON** contiene la specifica tecnica completa.

Include invece:
- metadata di citazione (`CITATION.cff`);
- documentazione descrittiva e introduttiva;
- esempi **non normativi**;
- riferimenti versionati alla specifica ZSE.

È pensato per:
- ricercatori,
- revisori,
- integratori,
- lettori che hanno accesso alla specifica completa.

---

## Fondamenti concettuali

ZSE si basa su tre vettori di controllo:

1. **Role Conditioning** — definizione del sottospazio semantico  
2. **Constraints Injection** — vincoli prescrittivi e proscrittivi  
3. **Output Formatting** — struttura sintattica verificabile

La formalizzazione completa, i vincoli normativi e le implicazioni operative
sono definiti **esclusivamente** nella specifica tecnica distribuita separatamente.

---

## 📚 Documentazione disponibile

- **Materiale descrittivo (EN):** `docs/en/`
- **Materiale descrittivo (IT):** `docs/it/`
- **Esempi non normativi:** `examples/`

---

## 🎯 Scopo della Specifica

La specifica ZSE ha tre obiettivi principali:

1. Definire ZSE come **disciplina ingegneristica** per il controllo inference-time degli LLM.  
2. Fornire una **base concettuale e normativa** per sistemi, agenti e tool compatibili.  
3. Costituire un **riferimento citabile** per lavori accademici e industriali.

---

## 🌍 Lingue

- Questo README è in **italiano**.
- Materiali descrittivi sono disponibili anche in **inglese**.

---

## 📜 Licenza

Il contenuto di questo repository è rilasciato sotto licenza  
**Creative Commons CC BY-NC-SA 4.0**.

La licenza **non implica** accesso alla specifica tecnica completa.

Vedi [`LICENSE`](LICENSE) per i dettagli.

---

## 👤 Autore

**Alberto Furnari**  
Senior System Engineer & AI Technical Lead  

- LinkedIn: https://www.linkedin.com/in/alberto-furnari-97695028  
- Newsletter: https://albertofurnari.substack.com
