# Zero-Shot Engineering — Public Overview (v1.1.0)

> ⚠️ **Scope notice**  
> This document is a **public, non-normative overview** of Zero-Shot Engineering (ZSE).  
> The **canonical technical specification** is distributed separately under controlled access.

---

## 0. Abstract

Zero-Shot Engineering (ZSE) is an approach to inference-time control of
autoregressive Large Language Models in zero-shot settings.

Rather than providing in-context examples, ZSE relies on **structured prompt design**
to restrict the semantic region in which a model operates.
This overview introduces the three conceptual control vectors commonly
associated with ZSE:

1. **Role Conditioning**
2. **Constraints Injection**
3. **Output Formatting**

Formal definitions, guarantees, and operational rules are specified
exclusively in the full technical specification.

---

## 1. Context (Descriptive)

In zero-shot conditions, LLMs often operate under high semantic ambiguity,
distributing probability mass across a large token support.

Commonly observed failure patterns include:

- semantic drift
- co-occurrence bias
- stylistic divergence
- hallucinated structure
- unstable formatting

ZSE addresses these issues conceptually by **reducing the effective freedom**
of the generation process through explicit contextual constraints.

---

## 2. Conceptual Control Vectors (Non-Normative)

The following elements describe the **conceptual building blocks**
commonly used in ZSE-style prompts.

### 2.1 Role Conditioning

Role conditioning consists in assigning an explicit functional role
to the model in order to narrow:

- the probable vocabulary
- the expected register and syntax
- the active semantic domain
- the associated patterns activated during training

**Illustrative example:**

```

Act as a Senior Technical Reviewer specialized in engineering documentation.

```

---

### 2.2 Constraints Injection

Constraints express **requirements or prohibitions** on the generated output.

- **Prescriptive constraints** indicate required elements or structure.
- **Proscriptive constraints** suppress entire categories of undesired output.

**Illustrative example (negative constraints):**

```

* Do not include greetings.
* Do not use colloquial tone.
* Do not add personal opinions.
* Do not propose rewrites.

```

These constraints conceptually reduce the space of admissible generations.

---

### 2.3 Output Formatting

Output formatting introduces a **structural expectation** for the response,
typically using a machine-verifiable format.

Common examples include:

- JSON
- Markdown with fixed sections
- Tables
- YAML

**Illustrative example:**

```

Output format:

* Markdown
* Three sections:

  1. Problem
  2. Analysis
  3. Conclusion

```

---

## 3. Observed Failure Patterns (Descriptive)

In practice, structured prompting approaches such as ZSE are commonly
used to mitigate:

- semantic drift
- co-occurrence bias
- stylistic drift
- hallucinated structure
- non-verifiable output

The formal treatment of these failure modes is provided
in the full technical specification.

---

## 4. Illustrative Prompt Structure

A commonly used high-level structure for ZSE-style prompts includes:

1. Role
2. Task
3. Constraints
4. Output format

**Illustrative template:**

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

This template is provided **for illustration only** and is not normative.

---

## 5. Minimal Illustrative Example

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

This document is a **partial and descriptive overview**.
It does not include:

- mathematical formalization
- log-probabilistic analysis
- normative constraint hierarchies
- advanced operational protocols

These elements are defined exclusively in the full ZSE technical specification,
distributed separately.

---

## 7. License

This document is released under **Creative Commons CC BY-NC-SA 4.0**.

Access to this file does **not** imply access to the full technical specification.
