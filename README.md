# Natural language processing course: `The Parse Force - Project 7`
# Register-sensitive machine translation with LLMs

This project investigates how large language models (LLMs) handle formality and register preservation in multilingual tasks. We analyzed translations from English into German and English into Slovene using different prompt strategies and evaluated the output with BLEU scores.

---

## Table of content

- [Dataset](#-dataset)
- [Translation Models](#-translation-models)
- [Prompting Strategies](#-prompting-strategies)
- [Evaluation Methods](#-evaluation-methods)
- [Results Summary](#-results-summary)
- [Credits](#-credits)

---
## Dataset

- **FAME-MT Corpus**: English-German parallel data annotated for formality.
- **Manual Slovene Translations**: Created by native speakers for this project.
- Total: 60 English source sentences (30 formal, 30 informal), translated into German and Slovene.

---

## Translation models

- GPT-4o (ChatGPT)
- DeepSeek
- Gemma

We tested each model using all four prompt strategies

---

## Prompting strategies
| Type        | Description |
|-------------|-------------|
| Explicit A  | Few-shot with role + clear task instructions |
| Explicit B  | Chain-of-thought reasoning with register identification |
| Implicit A  | Few-shot with examples only, no task description |
| Implicit B  | Zero-shot with minimal instruction |

---

## Evaluation methods
- **BLEU scores** using [`sacrebleu`](https://github.com/mjpost/sacrebleu) for lexical overlap

---

## Results summary
- GPT-4o performed best overall, especially with Explicit B prompts
- Register preservation was inconsistent across models
- Slovene outputs were more sensitive to prompt quality than German

---

## Credits
This project was developed as part of the class "Natural language processing" (UL-FRI) in 2024/25 by:
- Ines Karažija
- Isabell Furkert
- Lea Vodopivec
- Supervisor: Aleš Žagar

---

## License
This project is for academic/research purposes only.
