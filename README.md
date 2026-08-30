# Introduction

## Statistical Theory Question Answering Dataset

The Statistical Theory Question Answering (STQA) subset evaluates foundational knowledge across core theoretical domains, covering both general statistics and economic statistics. The dataset incorporates a diverse mix of item types—including single-choice, multiple-choice, true/false, and numerical calculation questions—paired with ground-truth answers and structured metadata (e.g., subject classification, difficulty tier, and reasoning rubrics). For public demonstration and format verification purposes, a representative sample of 50 curated questions per subject is provided in this repository.

### Data Format

Each record follows the JSON structure below:

```json
{
  "Question": "Question text...",
  "Options": ["A", "B", "C", "D"],
  "Answer": "C",
  "Metadata": {
    "index": 1,
    "subject": "Econometrics",
    "question_type": "conceptual",
    "question_format": "single_choice",
    "topic": "Introduction"
  }
}
```

- `Question` — the question text.
- `Options` — the list of choices (omitted for numerical questions).
- `Answer` — the correct answer (a letter, a combination of letters, `T`/`F`, or a numeric value).
- `Metadata.question_type` — `conceptual`, `calculation`.
- `Metadata.question_format` — `single_choice`, `multiple_choice`, `True_or_False`, or `numerical`.


## Statistical Practice Question Answering Dataset

The Statistical Practice Question Answering (SPQA) subset evaluates large language models on real-world statistical applications, policy enforcement, and practical survey operations.  The complete SPQA dataset is fully open-sourced.


## Usage & License

This dataset is provided for **academic research and educational purposes only**.


