# Zero-Shot Engineering — Public Specification (v1.0)

## 0. Abstract

Zero-Shot Engineering (ZSE) is a constraint-based framework for controlling autoregressive generation in zero-shot settings.  
Instead of providing examples, ZSE shapes the **semantic subspace** in which an LLM is allowed to operate through three control vectors:

1. **Role Conditioning**  
2. **Constraints Injection**  
3. **Output Formatting**

This specification defines the minimal structure of a ZSE-compatible prompt and the main failure modes it mitigates.

---

## 1. Context

In zero-shot conditions, LLMs operate under high semantic ambiguity and distribute probability across a large token support.  
Typical failure modes include:

- semantic drift  
- co-occurrence bias  
- stylistic divergence  
- hallucinated structure  
- unstable formatting

ZSE mitigates these issues by reducing:

- effective entropy of the conditional distribution  
- branching factor of the decoding trajectory  
- variance across generations  

---

## 2. Control Vectors

### 2.1 Role Conditioning

A role narrows:

- the probable vocabulary  
- the expected register and syntax  
- the active domain  
- the associated patterns learned during training  

**Example:**

```

Act as a Senior Technical Reviewer specialized in engineering documentation.

```

---

### 2.2 Constraints Injection

Constraints declare what the model must or must not output.

- **Prescriptive constraints:** require specific structure or elements.  
- **Proscriptive constraints:** suppress entire token families.

**Example (negative constraints):**

```

* Do not include greetings.
* Do not use colloquial tone.
* Do not add personal opinions.
* Do not propose rewrites.

```

This reduces the branching factor and limits semantic drift.

---

### 2.3 Output Formatting

The output format acts as a structural cage.

Examples:

- JSON  
- Markdown with fixed sections  
- Tables  
- YAML  

**Example:**

```

Output format:

* Markdown
* Three sections:

  1. Problem
  2. Analysis
  3. Conclusion

```

---

## 3. Failure Modes Mitigated

ZSE specifically addresses:

- **Semantic Drift**  
- **Co-occurrence Bias**  
- **Stylistic Drift**  
- **Hallucinated Structure**  
- **Non-verifiable Output**

---

## 4. Minimal Structure of a ZSE Prompt

A ZSE-compatible prompt contains:

1. **Role**  
2. **Task**  
3. **Constraints**  
4. **Output Format**

**Template:**

```

[ROLE]
Act as...

[TASK]
Analyze / Isolate / Evaluate...

[CONSTRAINTS]

* Do not...
* Do not...
* Use...

[OUTPUT FORMAT]
Markdown / JSON / other structured format

```

---

## 5. Minimal Example

```

Act as a Technical Reviewer.

Task:
Analyze the following text and identify logical inconsistencies only.

Constraints:

* Do not add greetings.
* Do not include personal commentary.
* Do not propose rewrites.

Output:
Markdown list, one bullet per inconsistency.

```

---

## 6. Scope and Limitations

This is a **public and partial specification**.  
It does not include:

- mathematical formalization  
- log-probabilistic analysis  
- advanced domain-specific patterns  
- a full operational toolkit  

The full version is available in the corresponding technical whitepaper.

---

## 7. License

This document is part of the *Zero-Shot Engineering — Public Specification* and is released under **CC BY-NC-SA 4.0**.
